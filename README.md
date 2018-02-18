## It's time for images to have a go at code clone detection!

![Vincent logo](https://ucl-crest.github.io/iwsc2018-vincent-web/images/logo.png)

We introduce a new code clone detection technique based on image similarity. The technique captures visual perception of code seen by humans in an IDE by applying syntax highlighting and images conversion on raw source code text. We compared two similarity measures, Jaccard and earth mover’s distance (EMD) for our image-based code clone detection technique. Jaccard similarity offered better detection perfor- mance than EMD. The F1 score of our technique on detecting Java clones with pervasive code modifications is comparable to five well-known code clone detectors: CCFinderX, Deckard, iClones, NiCad, and Simian. A Gaussian blur filter is chosen as a normalisation technique for type-2 and type-3 clones. We found that blurring code images before similarity computation resulted in higher precision and recall. The detection performance after including the blur filter increased by 1 to 6 percent. The manual investigation of clone pairs in three software systems revealed that our technique, while it missed some of the true clones, could also detect additional true clone pairs missed by NiCad.

### Vincent: an image-based code clone detection tool

Vincent is an open-source tool and can be downloaded here: [Vincent repo](https://bitbucket.org/chaiyong_ragkhitwetsagul/vincent/overview)

Note: The EMD library [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/) currently does not work with Ubuntu. I've found that it works with macOS. If you are running Vincent on Ubuntu, please comment the line `import emd`.

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

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/UCL-CREST/iwsc2018-vincent/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
