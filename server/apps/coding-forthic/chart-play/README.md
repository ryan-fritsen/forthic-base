An experiment in loading in a React chart via Forthic

Code Snippet sources:
- RF Warmups 2 for Main-Page nomenclature
- UAT-2 for JSX loading in the old style
- quadrant-play for HTML boilerplate (with tweaks)

Some observations
- UAT-2 
  - Runs the React component from browser.forthic, via RUN-JS.
  - Main.forthic invokes JSX via text/babel script type:
  
                <script type="text/babel">
                    {{ jsx_util }}
                    {{ jsx }}
                </script>

Phrases Needed:
- RUN-JS
- 