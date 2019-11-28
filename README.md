# bibsdb/projector-screen

Supplies a slide template for playing projector-screen videos. This bundle uses ProjectorScreen's js player: https://github.com/projector-screen/player.js/

## Installation

Add the git repository to "repositories" in `composer.json`.

<pre>
"repositories": {
    "bibsdb/projector-screen-bundle": {
      "type": "vcs",
      "url": "https://github.com/bibsdb/projector-screen-bundle"
    },
    ...
}
</pre>

Require the bundle with composer.

<pre>
composer require bibsdb/projector-screen-bundle
</pre>

Enable the bundle in `AppKernel.php`, by adding BibsdbProjectorScreenBundle to $bundles.

<pre>
new Bibsdb\ProjectorScreenBundle\BibsdbProjectorScreenBundle()
</pre>

Run bibsdb:core:templates:load command to load the template in the installation.

<pre>
bin/console bibsdb:core:templates:load
</pre>

Enable the template in the administration.

## Ads and controls

To avoid ads and video controls, the shared video has to come from a user
that has disabled the options at projector-screen.com. To do it yourself, you need to have
at least a PLUS account (https://projector-screen.com/plus).
