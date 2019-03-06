Contributing
============

# Important notes

Here are some important notes before you contribute to Certificationy Symfony Pack:

* For legal reasons, you *MUST* have never passed the Symfony certification yet,
* All questions existing in Certificationy are not copied from a certification exam,
* You are not allowed to use the questions from the [Unofficial self-study guide](https://leanpub.com/symfony-selfstudy).

# Add questions

The official SensioLabs Symfony Certification contains 75 randomly chosen questions and is 90 minutes long. The examination covers the following topics:

* PHP
* HTTP
* Architecture
* Standardization
* Bundles
* Controllers
* Routing
* Twig
* Forms
* Validation
* Dependency Injection
* Security
* HTTP Caching
* Command Line Interface
* Automated testing
* Miscellaneous (error handling, code debugging)

from [Official Symfony certification](https://certification.symfony.com/).

You can add questions to each category. There are three types of questions:

* True/false questions
* Single answer questions
* Multiple answers questions

*There are no open questions or any lines of code to write.*

To contribute to the Symfony Pack, you can add questions in each category in YAML:

```yaml
-
    question: 'What is the prefix of environment variables used by Symfony?'
    answers:
        - {value: "SYMFONY__", correct: true}
        - {value: "SF__",      correct: false}
        - {value: "SYMFONY-",  correct: false}
        - {value: "SF-",       correct: false}
```

Check if the question is not present, to avoid duplications.

Finaly, validate your YAML files: you can use the built-in command of Symfony:

```bash
$ php app/console lint:yaml /path/to/your/yaml/file.yaml
```
