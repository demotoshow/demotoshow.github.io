# Abstract 

Neural sequence-to-sequence models are well established for applications which can be cast as mapping a single input sequence into a single output sequence. In this work, we focus on one-to-many sequence transduction problems, such as extracting multiple sequential sources from a mixture sequence. We extend the standard sequence-to-sequence model to a novel conditional multi-sequence model, which explicitly models the relevance between multiple output sequences with the probabilistic chain rule. We take speech data as a primary test field to evaluate our methods since the observed speech data is often composed of multiple sources due to the nature of the superposition principle of sound waves. Experiments on several different tasks including speech separation and multi-speaker speech recognition show that our conditional multi-sequence models lead to consistent improvements over the conventional non-conditional models.

# Motivation
![image](https://user-images.githubusercontent.com/66230088/83373061-30a81d80-a395-11ea-81ab-ef2b6af06f97.png)
For clarity, we refer our methods as Conditional Chain model, combining both the serial mapping and parallel mapping with the probabilistic chain rule. Simultaneous modeling for these two paradigms not only makes the framework more flexible but also encourages the model to automatically learn the efficient relationship between multiple outputs.




# Proposed methods
![image](https://user-images.githubusercontent.com/66230088/83373798-9eeddf80-a397-11ea-9806-67c02b281cde.png)

our proposed structure provides a solution to the variable and unknown output number issues.

# Speech sepration samples 
WSJ0-2mix & 3mix are used by use to remix some 4 speaker and 5 speaker mixtures.

## WSJ0-4mix Sample 1 (2Female & 2Male)
### Mixture and separted spectrograms
![image](https://user-images.githubusercontent.com/66230088/83374674-5126a680-a39a-11ea-8ede-916fb812aec0.png)
### Mixed audio
<audio id="4mix_0" controls="" preload="none">
<source id="wav" src="./audio/2_True_mix.wav">
</audio>
### Separated sources
<audio id="4mix_0_pre0" controls="" preload="none">
<source id="wav" src="./audio/2_01c_pre.wav">
</audio>
<audio id="4mix_0_pre1" controls="" preload="none">
<source id="wav" src="./audio/2_01e_pre.wav">
</audio>
<audio id="4mix_0_pre2" controls="" preload="none">
<source id="wav" src="./audio/2_20c_pre.wav">
</audio>
<audio id="4mix_0_pre3" controls="" preload="none">
<source id="wav" src="./audio/2_204_pre.wav">
</audio>

## WSJ0-4mix Sample 2 (1Female & 3Male)
### Mixture and separted spectrograms
![image](https://user-images.githubusercontent.com/66230088/83375499-078b8b00-a39d-11ea-8155-021961dd6b1f.png)
### Mixed audio
<audio id="4mix_1" controls="" preload="none">
<source id="wav" src="./audio/1_True_mix.wav">
</audio>
### Separated sources
<audio id="4mix_1_pre0" controls="" preload="none">
<source id="wav" src="./audio/1_22g_pre.wav">
</audio>
<audio id="4mix_1_pre1" controls="" preload="none">
<source id="wav" src="./audio/1_052_pre.wav">
</audio>
<audio id="4mix_1_pre2" controls="" preload="none">
<source id="wav" src="./audio/1_423_pre.wav">
</audio>
<audio id="4mix_1_pre3" controls="" preload="none">
<source id="wav" src="./audio/1_442_pre.wav">
</audio>

## WSJ0-4mix Sample 3 (3Female & 1Male)
### Mixed audio
<audio id="4mix_2" controls="" preload="none">
<source id="wav" src="./audio/9_True_mix.wav">
</audio>
### Separated sources
<audio id="4mix_2_pre0" controls="" preload="none">
<source id="wav" src="./audio/9_053_pre.wav">
</audio>
<audio id="4mix_2_pre1" controls="" preload="none">
<source id="wav" src="./audio/9_441_pre.wav">
</audio>
<audio id="4mix_2_pre2" controls="" preload="none">
<source id="wav" src="./audio/9_443_pre.wav">
</audio>
<audio id="4mix_2_pre3" controls="" preload="none">
<source id="wav" src="./audio/9_444_pre.wav">
</audio>

## WSJ0-5mix Sample (2Female & 3Male)
### Mixture and separted spectrograms
![image](https://user-images.githubusercontent.com/66230088/83378945-4a9f2b80-a3a8-11ea-87b0-7fc215bee890.png)
### Mixed audio
<audio id="5mix_0" controls="" preload="none">
<source id="wav" src="./audio/0_True_mix.wav">
</audio>
### Separated sources
<audio id="5mix_0_pre0" controls="" preload="none">
<source id="wav" src="./audio/0_22g_pre.wav">
</audio>
<audio id="5mix_0_pre1" controls="" preload="none">
<source id="wav" src="./audio/0_442_pre.wav">
</audio>
<audio id="5mix_0_pre2" controls="" preload="none">
<source id="wav" src="./audio/0_423_pre.wav">
</audio>
<audio id="5mix_0_pre3" controls="" preload="none">
<source id="wav" src="./audio/0_050_pre.wav">
</audio>
<audio id="5mix_0_pre4" controls="" preload="none">
<source id="wav" src="./audio/0_052_pre.wav">
</audio>

