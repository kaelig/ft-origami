## This is a gh-pages branch

Please visit http://origami.ft.com to view the site

## Building

Since this is a GitHub pages site, built CSS bundle must be committed to the repository.  We store it in `buildcache` to avoid any confusion - files in the `buildcache` directory should not be edited.  To regenerate them, use Grunt:

1. Clone the repository
1. Ensure `grunt-cli` is installed globally by checking it's listed with `grunt --version`.  If it's not, install with `npm install -g grunt-cli`.
1. Run `npm install`
1. Edit main.scss as desired
1. Run `grunt`

## Viewing locally

1. Install Jekyll `gem install jekyll`
1. Install Jekyll redirect gem `gem install jekyll-redirect-from`
1. Run `jekyll serve --watch --baseurl=''` and view on http://localhost:4000/
1. Run `grunt watch` in parallel if you're editing styles

## Documentation style guide
This guide is based on https://jacobian.org/writing/great-documentation/. It exists as guidance to help keep our documentation consistent.

### Types of documentation
There are three types of documentation:

1. **Step by step tutorials**: These are the on-ramp for our project. Users should be able to follow one of our step-by-steps and achieve success within 30 minutes. These live in this repo (ft-origami).
1. **Topic guides**: We don't have these yet. They should cover topics in comprehensive detail. They include information that would be too dense for a step-by-step.
1. **Reference**: The Origami Spec is the container for general conventions for Origami components. Each component has it's own reference documentation too, found in its readme, JSdoc and Sassdoc.

### Style
We assume good grammar and proper spelling is already a given so it's not in this list. The Origami Spec is a [normative specification](https://www.w3.org/TR/qaframe-spec/) and follows the conventions of normative specifications. For our other documentation (tutorials, topic guides and readmes) we use a much less formal tone. They should be informative, but breezy and conversational.

1. Be conversational
  - Use contractions: "we're" over "we are"
  - Starting sentences with conjunctions like 'but' or 'so' is allowed
1. Prefer "we" to "I"
  - **good**: "we recommend you do X"
  - **bad**: "I recommend you do X"
1. Use the active voice. If you need help with this one, use [http://www.hemingwayapp.com/](http://www.hemingwayapp.com/)
  - **good**: "we recommend you do X"
  - **bad**: "it is recommended you do X"
1. Omit fluff. Avoid qualifiers like "pretty", "mostly", "probably"
1. Prefer short sentences to long sentences
1. Use British English
  - **good**: organise, favour
  - **bad**: organize, favor
1. Avoid metaphors or turns of phrase that non-native English speakers may not be familiar with
  - **good**: "this site has everything you need to know"
  - **bad**: "this site is a one stop shop for Origami"
1. [Avoid "simply" and other words that trivialise concepts and ideas that might not be trivial](https://css-tricks.com/words-avoid-educational-writing/)
1. Structure documentation for skim readers
  - Code variables go in `back-ticks`
  - Use tables
  - Use asides for extra tidbits
  - Use **strong** and _emphasis_ where appropriate
  - Use lists
  - Break things up with informative headings
1. Always capitalise Origami when referring to the product
1. Never capitalise modules
  - **good**: o-techdocs, o-component
  - **bad**: O-techdocs, O-Techdocs
1. Always capitalise Origami services
  - **good**: the Polyfill Service, the Build Service
  - **bad**: the polyfill service, the build service
