# Sort Smart

AI Final Project by Pranav

AI Final Project prototype for [United Nations SDG 12](https://sdgs.un.org/goals/goal12).

## Run the demo

Download and open SortSmart.html in a modern web browser. The entire interface and model run
offline. The project uses HTML, CSS and JavaScript and requires no API key,
server or external dependency.

### How it works

The prototype trains a multinomial Naive Bayes classifier in the browser from
48 authored examples, 12 each for four categories. It uses term frequencies
with add-one smoothing and normalizes category log-likelihoods to relative
scores. It abstains if there are no recognized terms, the highest score is below
0.53, or the margin is below 0.17. Specific special-item words bypass the score
and trigger a local collection lookup suggestion.

### Try the key interaction

1. Try the cardboard box, banana peel and ceramic mug suggestions.
2. Try “laptop battery” to see special collection handling.
3. Type “blue thing” and submit to see what happens when vocabulary is missing.
4. Review the five most recent checks and choose **Clear** to remove that history.

### Scope

Results are educational guidance. Consult local collection rules. Relative
scores have not been validated as confidence estimates. Recent checks stay in
browser memory until the page reloads or the history is cleared.

## License

This source package includes an MIT license.

## Submission files

- [Application source](SortSmart.html)
- [Project report and screenshots](SDG_SortSmart_Pranav.pdf)
- [Download the source archive](SortSmart-Source.zip)
