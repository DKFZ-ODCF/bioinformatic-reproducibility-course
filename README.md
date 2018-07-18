# Conda for Convenience and Reproducibility

A short presentation and course given for a group of molecular biotechnology master students in Heidelberg, Germany.

Have a look at https://dkfz-odcf.github.io/conda-course/ to see the presentation.

## Build Instructions

* Clone the repository
  ```bash
  git clone https://github.com/DKFZ-ODCF/conda-course.git
  ```

* Build the presentation
  ```bash
  cd conda-course
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

 * 1.0: Held 18th July 2018