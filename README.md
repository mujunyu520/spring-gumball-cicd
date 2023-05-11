# spring-gumball ci/cd example cha


## CI Workflow
For the examination, we need to pull the spring-gumball from the professor's repository (Lab 10) into the personal GitHub Repo as public.
and we got to make a workflow under this repo
![WX20230511-130803](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/d9d1b432-6e40-4d36-9b1a-3ca5cb53ddc1)


![gradle-1](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/5338fff0-c4c7-4ee5-ad4e-2cfac5144ce4)

and make sure your building tool was raelly set up

![image](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/aa35d69d-3ccc-4004-b631-38109b419011)

after that make workflow run the gradle.yaml provide by prof




## Cd workflow

Foe CD workflow exercise, we need to set up the GKE as below picture And then, we create the kubernetes cluster.
![cd workflow-1](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/43c10485-ffa1-43e4-b6ae-33c906a69bac)

![cd workflow-3](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/208deed4-5c51-4956-a163-39dab0ac4ec0)
![cd workflow-4](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/66f24868-e829-49d5-9ae4-99bc6a846756)

since I am still working on my defult porjcet ID , then I neeed to create a cmpe172 to match with lab requirement.

![cd workflow-5](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/ff0e55b0-c5e5-4455-aa99-ebabda33af35)
![cd workflow-6](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/0d2da414-5aac-4fae-b665-71239ade3240)

then we need to add another service accounts by naming spring-gumball
![cd workflow-7](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/6b8e4018-aedd-40af-9d46-71fa2981bb6f)



After this step, next set a json key for connectting to gcloud.
![cd workflow-8](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/ba616bd1-2bb9-489c-bd63-14675a729923)

![cd- workflow-10](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/6e9bb8e0-9eda-4d5a-95ad-0c05cca7a971)

then go to iam to make another role for the project!

![cd-workflow9](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/eda8b60f-8257-41c9-bd2a-050ed8a9ff2a)



then we got to github secrets and vairbles seciton to set up GKE_PROJECT and GKE_SA_KEY 

![cd workflow-12](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/eab440ae-2a5b-4972-b126-27af89252ba9)


next , copy the google.yml configuration from the lab10  google.yml runs without error

![cd workflow-14](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/3f4812dd-c18b-4815-a7c1-07a9a1ab26b8)



then we need to release the spring-gumball projects

![cd workflow-15 release](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/e326b03d-d819-424e-85e8-a085650947de)



after we release we can notice it is building everhting by itself.

![cd-workflow-16building](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/b7d047a3-33cb-469d-8273-fa5790dfaebb)



release version build without any error.

![cd workflow-17 builed](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/0887cb82-83b4-492e-a457-c8820848cf52)


after set up everthing we can go back to GCP, we can find out our services are really running 

![cd workflow-18 deployment](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/50dd51e5-2ff6-4332-800b-f434cc2d09f5)

![cd workflow-19 service](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/48aab0b4-3d67-4b5a-9c49-d12b7c75553c)




then we need create ingress for external port for hte spring gumbal

![cd workflow-18 ingress](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/be36cdde-eda1-40d5-9e31-b9739afa1a10)



YES it shows up spring gumball GKE version here:
![cd workflow-19](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/2a2095af-3a6a-45f0-83ce-36cbc910c709)



fullscreen

![full screen](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/04e9c21d-e53f-4b82-8617-2e323bb7aaab)


endhere

