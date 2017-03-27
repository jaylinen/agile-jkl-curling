# Gofore Microservices Training

Welcome to the Gofore Microservices Training package! This repository contains material for several days worth of
presentations.

All contributions are welcome. Before contributing, please read the [contribution guidelines](/doc/contribution_guidelines.md)
and the [markdown styleguide](/doc/markdown_styleguide.md). Let others know what you are working on, and try to make
smaller changes, instead of hoarding edits for a whole week.

For more information, see the Confluence page ["Pilvikoulutuspaketti"](https://extra.gofore.com/confluence/display/GOF/Pilvikoulutuspaketti)
or join the Slack channel [#pilvikoulutus-2017](https://gofore.slack.com/messages/pilvikoulutus-2017/).

## Prerequisites

Reveal.js is included as a git submodule so that it can easily be updated. Therefore, remember to initialize the git
submodules before doing anything else:

    git submodule update --init --recursive

## Starting the presentation

To start the presentation, run the following command in the root of the repository:

    ./start_presentation.sh

Now, you can access the presentation slides with your browser by going to:

    http://localhost:8000

To show the speaker notes, just press the `s` key while you have a presentation open.

To view the presentation in fullscreen mode, press `f`.

To view the overview mode, press `Esc` or `o`.

For more details, refer to the [Reveal.js documentation](https://github.com/hakimel/reveal.js/).

## Exporting to PDF

There are three ways to export the PDFs. You can either use the provided script [export_pdfs.sh](export_pdfs.sh) to
export all presentations to pdf, use Reveal.js's own export functionality, or the [decktape tool](https://github.com/astefanutti/decktape).
There can be some style issues with Reveal.js's own export functionality. Decktape on the other hand seems to generate
the PDFs without style issues.

### Provided script

The provided script uses decktape and Ghostscript to export the pdfs and combine them into one. Just run:

    ./export_pdfs.sh

### Reveal.js export

Reveal.js recommends using Google Chrome or Chromium for exporting to PDF.

1. Open your presentation with print-pdf included in the query string, e.g.,. `http://localhost:8000/microservices-intro/?print-pdf`.
1. Open the in-browser print dialog (CTRL/CMD+P).
1. Change the **Destination** setting to **Save as PDF**.
1. Change the **Layout** to **Landscape**.
1. Change the **Margins** to **None**.
1. Enable the **Background graphics** option.
1. Click **Save**.

For more details, refer to <https://github.com/hakimel/reveal.js/#pdf-export>

### Decktape

To convert a presentation by running dectape within a Docker container, run:

    docker run --rm --net=host -v `pwd`:/slides astefanutti/decktape http://localhost:8000/microservices-intro/ slides.pdf

For more details, refer to [decktape's instructions](https://github.com/astefanutti/decktape).

## Installation (for development and content creation)

Next, you need to install the npm dependencies:

    npm install

Finally, you can start a local server which serves the static presentation slides:

    gulp

Now, you can access the presentation slides with you browser by going to:

    http://localhost:3000

## Creating or updating presentation slides

For creating or updating presentation slides, refer to the [modules README.md](modules/README.md) file.
