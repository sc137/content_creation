# Web Content Creation Workshop

Sable Cantus

This presentation is a training tool that will be used in workshops with Rio Hondo College faculty and staff to help them start rewriting content for their part of the campus website.

This project uses a simple markdown text file and pandoc to convert to a slideshow.

I was using slidy initially - it is fast and simple.

    pandoc -t slidy -s content_creation.md -o index.html --template slidy.template

The file slidy.template calls out the assets/slidy.css so you can easily customize the look and feel.

I switched to reveal.js because it just looks **so** good.

    pandoc -t html5 --template=revealjs.template --standalone --section-divs --variable theme="beige" --variable transition="linear" content_creation.md -o index.html

Please feel free to use these resources and materials in your own training.
