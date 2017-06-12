Pre-commit hook for Imageoptim-cli For Mac  
==========================================

This is a imageoptim-cli hook for [pre-commit](https://github.com/pre-commit/pre-commit). This optimised images on commit.


### Using styleint with pre-commit

- To use this you first need to install pre-commit(see links below).
- Then create a pre-commit config file and also a stylelint config file in the root of your project.
- Run `pre-commit install` from the root of your project

Finally add this to your `.pre-commit-config.yaml`:

```yaml
   -   repo: https://github.com/awebdeveloper/pre-commit-imageopti
       sha: '' # Use the sha or tag you want to point at like 0.0.1
       hooks:
       -   id: imageoptim
           additional_dependencies: ['imageoptim-cli']
 ```

 Now everytime you commit a png/jpg file. It will run imageoptim-cli on this and optimise the file.

 ### Links
 - For pre-commit: see https://github.com/pre-commit/pre-commit
 - For ImageOptim-CLI: see https://github.com/JamieMason/ImageOptim-CLI/


