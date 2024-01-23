---
permalink: /
title: "Hello! I'm Seonho Kim!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
    .project-content {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .project-content .project-text,
    .project-content .project-image {
        width: 100%;
    }
</style>
<style>
    @media screen and (min-width: 768px) { 
        .project-content {
            flex-direction: row; /* This reverses the order of flex items */
        }
        .project-content .project-text {
            flex: 1;
            padding-right: 20px; /* Adjust padding to the left of the text for separation */
        }
        .project-content .project-image {
            max-width: 300px;
          
        }
    }
           .justified-text {
            text-align: justify;
        }
</style>


I am a fifth-year Ph.D. student at the Ohio State University, working with [Prof. Kiryung Lee](https://u.osu.edu/kiryung). Prior to that, for my MS and BS degrees, I was fortunate to be advised by [Prof. Songnam Hong](https://sites.google.com/view/snlab) at Ajou University in South Korea. My research interests span the algorithmic foundations in the fields of data science, machine learning, optimization, and signal processing.







<a id="research_summary"></a>
## Research Summary

### Parameter-Efficient Fine Tuning using Trace norm regularization

<div class="project-content">
    <div class="project-text">
        <p class="justified-text">Low-Rank Adaptation (LoRA) is a representative, parameter-efficient fine-tuning method for large pre-trained models in downstream tasks. To enhance LoRA's parameter efficiency, we propose a novel pruning technique that utilizes the trace norm (also referred to as the nuclear norm) with matrix factorization. We demonstrate that our method outperforms baseline algorithms, including LoRA and AdaLoRA, on the GLUE benchmark dataset, using a fewer number of parameters. This work is still ongoing for various benchmark datasets, and the work is undergoing.
        </p>
    </div>
    <div class="project-image">
        <figure>
            <img src='/images/TraceLoRA_figure.png' style='width:300px;' alt='TraceLoRA'>
            <figcaption>An illustration of a low-rank matrix update using trace norm, where the updated matrix exhibits sparse singular values.</figcaption> <!-- Caption for the first image -->
        </figure>
    </div>
</div>



### Robust Phase Retrieval via iterative Gauss-Newton Method

<div class="project-content">
    <div class="project-text">
        <p class="justified-text">Phase Retrieval recovers a signal from the absolute value of its linear measurements, which arises in signal and imaging processing. We proposed an iterative Gauss-Newton method for phase retrieval in outlier scenarios and demonstrated that a linear program can solve a step of the Gauss-Newton method. Furthermore, we established that in outlier scenarios, the method converges to the ground-truth signal at a linear rate with near-optimal sample complexity with high probability. Lastly, we demonstrate that our proposed methods are computationally efficient and exhibit superior performance compared to the baseline algorithms. This work is to appear in
        <a href="https://2024.ieeeicassp.org/">ICASSP 2024</a>
        </p>
    </div>
    <div class="project-image">
        <figure>
            <img src='/images/groundtruth.png' style='width:30%;' alt='Project Image 1 Description'>
            <img src='/images/init_ours.png' style='width:30%;' alt='Project Image 2 Description'>
            <img src='/images/recover_ours.png' style='width:30%;' alt='Project Image 3 Description'>
            <figcaption>Image recovery of our algorithm: Left is true digit; middle is initialization; right is recovered image.</figcaption> 
            <!-- Caption for the first image -->
        </figure>
        <figure>
            <img src='/images/groundtruth.png' style='width:30%;' alt='Project Image 4 Description'>
            <img src='/images/init_base.png' style='width:30%;' alt='Project Image 5 Description'>
            <img src='/images/recovered_base.png' style='width:30%;' alt='Project Image     Description'>            
            <figcaption>Image recovery of baseline algorithm: Left is true digit; middle is initialization; right is recovered image.</figcaption> 
            <!-- Caption for the second image -->
        </figure>
    </div>
</div>

----

### Max-Affine Regression
<div class="project-content">
    <div class="project-text">
        <p class="justified-text"> 
            Max-affine regression recovers parameters in the max-affine function from its observations, which arise in statistics, economics, and machine learning. However, max-affine regression is challenging due to its non-convexity. We proposed two efficient algorithms.
        </p>
        <ul>
            <li>
                <strong>First Order Methods:</strong> Gradient Descent (GD) and Stochastic Gradient Descent (SGD) are efficient and popular algorithms for solving non-convex optimization problems. We unveiled the effectiveness of first-order methods for max-affine regression through rigorous theoretical results. We demonstrate that first-order methods, when initialized near the ground-truth parameters, can solve the max-affine regression problem with linear convergence. The sample complexity is linear in terms of dimension, and polynomial in terms of certain geometrical parameters and the number of affine functions, with a high probability.
                <a href="https://arxiv.org/abs/2308.08070">Read More</a>
            </li>
            <li>
                <strong>Convex Program:</strong> We proposed a convex program to solve max-linear regression, which is a special case of max-affine regression. We show that this convex program can solve the max-affine regression problem with sample complexity comparable to the best-known results. Furthermore, we have demonstrated that our iterative version of the convex program is robust in outlier scenarios.
                <a href="https://ieeexplore.ieee.org/abstract/document/10381831">Read More</a>
            </li>
        </ul>
    </div>
   <div class="project-image">
        <figure>
            <img src='/images/approxwages.png' style='width:300px;' alt='Max-affine regression on mean weakly wages data'>
            <figcaption>Max-affine model learned by SGD on mean weekly wages data</figcaption> <!-- Caption for the first image -->
        </figure>
        <figure>
            <img src='/images/approxihouse.png' style='width:300px;' alt='Max-affine regression on Boston house prices data'>
            <figcaption>Max-affine model learned by SGD on Boston house prices data</figcaption> <!-- Caption for the second image -->
        </figure>
    </div>
</div>






<!-- # Research Highlights

I am broadly intrested in the application and theoretical aspects in the fields of machine learning, optimization, signal processing and wireless communication. During Ph.D, I have mainly two folds research directions: 1. I work on developing scalable and efficient algorithms with theoretical guarantees for non-trivial statistical models. My main questions focus on that "how many data does the algorithm require for successful estimating some models?" and "Can the algorithm learn the model with high probability"? 2. I'm also working on the algorithm for promoting the sparsity in the model for efficient learning. -->

<!-- low-rank matrice estimation and update in fields of efficient learning 

analysis in statstical models via mathematical tools of probability, linear algebra, and optimization; 2. For example, a fundamental question is that when we estimate a non-linear statistcal model using observations (supervised learning), how many observations do we need for the successful estimation? 2. I have been working  -->






<!-- ======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons.  -->
<!-- 
Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
