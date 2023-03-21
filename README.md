image: ruby:2.7

pipelines:
  branches:
    master:
    - parallel:
      - step:
          name: Test
          script:
            - echo "this id running pipeline"
            - pwd 
      - step:
          name: Lint code
          script:
            - echo "this id running pipeline 2"
            - pwd
