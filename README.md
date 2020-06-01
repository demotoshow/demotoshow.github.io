## Abstract 

Neural sequence-to-sequence models are well established for applications which can be cast as mapping a single input sequence into a single output sequence. In this work, we focus on one-to-many sequence transduction problems, such as extracting multiple sequential sources from a mixture sequence. We extend the standard sequence-to-sequence model to a novel conditional multi-sequence model, which explicitly models the relevance between multiple output sequences with the probabilistic chain rule. We take speech data as a primary test field to evaluate our methods since the observed speech data is often composed of multiple sources due to the nature of the superposition principle of sound waves. Experiments on several different tasks including speech separation and multi-speaker speech recognition show that our conditional multi-sequence models lead to consistent improvements over the conventional non-conditional models.

## Motivation
<img src="https://user-images.githubusercontent.com/66230088/83373061-30a81d80-a395-11ea-81ab-ef2b6af06f97.png" width = "730" height = "250" alt="" align=center />
For clarity, we refer our methods as Conditional Chain model, combining both the serial mapping and parallel mapping with the probabilistic chain rule. Simultaneous modeling for these two paradigms not only makes the framework more flexible but also encourages the model to automatically learn the efficient relationship between multiple outputs.

## Proposed methods
<img src="https://user-images.githubusercontent.com/66230088/83373798-9eeddf80-a397-11ea-9806-67c02b281cde.png" width = "730" height = "300" alt="" align=center />

our proposed structure can provide a solution to the variable and unknown output number issues.

## Speech sepration samples 
WSJ0-2mix & 3mix are used by use to remix some 4 speaker and 5 speaker mixtures.

#### WSJ0-4mix



Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/demotoshow/demotoshow.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
