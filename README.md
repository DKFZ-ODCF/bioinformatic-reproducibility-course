# Reproducibility in Bioinformatics

A short presentation (1/2 h) or course (probably 1.5 h) given for a group of molecular biotechnology master students in Heidelberg, Germany.

Have a look at https://dkfz-odcf.github.io/bioinformatic-reproducibility-course/ to see the presentation.

## Build Instructions

* Clone the repository
  ```bash
  git clone https://github.com/DKFZ-ODCF/bioinformatic-reproducibility-course.git
  ```

* Build the presentation
  ```bash
  cd bioinformatic-reproducibility-course
  ./gradlew asciidoctor
  ```

* Find the HTML5 and PDF products in the `build/` directory.

## Publishing GH Pages

The repo uses the [gradle-git-publish](https://github.com/ajoberstar/gradle-git-publish) plugin to publish an AsciiDoctor document to Github Pages.

You need a personal authentication token from Github. Go to your profile image (top-left) and choose "settings" and on the right select "developer settings". Proceed to "Personal access tokens" and or choose a token that has the ticks below "repo" and "admin:repo_hook" set.

You can publish your changes to the `gh-pages` branch with

```bash
./gradlew gitPublishPush
```

## Versions

 * 2.x.y: To be held on the 6th of March, 2019
 * 1.0.0: Held 18th July 2018
 
## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.