---
title: 'Number of moves to solve the Tower of Hanoi and its 2 variants'
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin


# Author notes (optional)
author_notes:
  - 'me'


date: '2021-12-21T13:38:00Z'
doi: 'https://doi.org/10.6084/m9.figshare.17091965.v4'

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: In *figshare*
publication_short: In *figshare*

abstract: We describe the minimal number of moves required to solve the traditional Tower of Hanoi game, the adjacent pegs variant, and the Cyclic Hanoi variant, by using recurrent relations and generating functions.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://figshare.com/articles/journal_contribution/Moves_required_to_solve_Tower_of_Hanoi_and_2_variants_pdf/17091965'
url_code: ''
url_dataset: ''
url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

If we denote {{< math >}}$a_n${{< /math >}} as the optimal number of moves to solve the puzzle with {{< math >}}$n${{< /math >}} pegs, {{< spoiler text="The recurrence relation for the classical variant is" >}} {{< math >}}$a_n=2a_{n-1}+1${{< /math >}} {{< /spoiler >}}

{{< spoiler text="The recurrence relation for the adjacent pegs variant is" >}} {{< math >}}$a_n=3a_{n-1}+2${{< /math >}} {{< /spoiler >}}

For the cyclic variant, we additionally define {{< math >}}$b_n${{< /math >}} as the number of moves required to move {{< math >}}$n${{< /math >}} pegs to its next clockwise peg.

{{% callout note %}}
{{< math >}}$a_n$ is *not* 2$b_n$. You can verify with the case $n=2$, with $a_2=7$ and $b_2=5$ (try it!){{< /math >}}
{{% /callout %}}

{{< spoiler text="The recurrence relation for the cyclic variant is" >}}{{< math >}} $\left \{
    \begin{array}{l}
      a_n=2a_{n-1}+b_{n-1}+2\\
      b_n=2a_{n-1}+1
    \end{array}
  \right.\\
  \Rightarrow a_n=2a_{n-1}+b_{n-1}+2=2a_{n-1}+(2a_{n-2}+1)+2=2a_{n-1}+2a_{n-2}+3.$
{{< /math >}}{{< /spoiler >}}

{{% callout note %}}
Try thinking about the recurrence relation of these variants when there are more than {{< math >}}$3${{< /math >}} rods-
{{% /callout %}}

For a detailed explanation and illustrations, please refer to [the article](https://figshare.com/articles/journal_contribution/Moves_required_to_solve_Tower_of_Hanoi_and_2_variants_pdf/17091965).
