# Knowledge Pixels Slides

Run local HTTP server:

    $ python -m http.server

Make PDF:

    $ docker run --rm -t -v $(pwd)/_pdf:/slides -v $(pwd):/home/user astefanutti/decktape /home/user/ds-pilot-editor-info.html /slides/slides.pdf

See: https://4comprehension.com/github-actions-reveal-js-and-automating-pdf-conversion/
