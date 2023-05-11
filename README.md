# spring-gumball ci/cd example

## CI Workflow
For the examination, we need to pull the spring-gumball from the professor's repository (Lab 10) into the personal GitHub Repo as public.
and we got to make a workflow under this repo
![gradle-1](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/e5677516-8cfc-4a01-88d6-b7c815befa39)


and make sure your building tool was raelly set up

![image](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/2e904c96-0dcd-4a27-a140-c3118fe2e569)

after that make workflow run the gradle.yaml provide by prof

![gradle-2](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/fb8d1cfb-e883-4a39-b2fa-8b5e8ecb680a)


## Cd workflow

Foe CD workflow exercise, we need to set up the GKE as below picture And then, we create the kubernetes cluster.
![cd workflow-1](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/b3d09532-fd55-4f5d-b092-3eed4d8e2a4e)
![cd workflow-3](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/8ab65b93-d36c-4672-afa8-1c6bf2ddfba4)
![cd workflow-4](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/170b962b-bc78-4ffa-8201-40a99d9d5915)

since I am still working on my defult porjcet ID , then I neeed to create a cmpe172 to match with lab requirement.
![cd workflow-5](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/8a252d9b-0ac5-4306-a19c-f2bcdec88789)
![cd workflow-6](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/b567be1c-be99-45c7-b104-7f4a78075771)

then we need to add another service accounts by naming spring-gumball

![cd workflow-7](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/b68f9122-84d2-4538-a99e-8530bfe4720d)


After this step, next set a json key for connectting to gcloud.
![cd workflow-8](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/58f69912-cf41-493d-8f02-938a8c818b13)
![cd- workflow-10](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/ba83c9a3-8555-47cc-9568-8eeb39964909)

then go to iam to make another role for the project!

![cd-workflow9](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/edd9c531-bc80-4735-a4c6-2ce368c555dd)


then we got to github secrets and vairbles seciton to set up GKE_PROJECT and GKE_SA_KEY 

![cd workflow-12](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/55ac12ae-467d-4539-92c0-9ddd90b9cf55)

next , copy the google.yml configuration from the lab10 
![image](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/eefaf3f6-1cf5-4266-91b9-a8ebc722a29a)

google.yml runs without error
![cd workflow-14](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/84414158-d304-461c-afb8-4ccc30911dc4)



then we need to release the spring-gumball projects


![cd workflow-15 release](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/fd356340-5a2f-4df7-bde8-26ea03c3ce0c)

after we release we can notice it is building everhting by itself.

![cd-workflow-16building](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/e6d0a087-c2b0-45dc-8496-eef65638dcfe)


release version build without any error.

![cd workflow-17 builed](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/31fcc01d-dfdf-41c7-b054-5fab44614620)


after set up everthing we can go back to GCP, we can find out our services are really running 

![cd workflow-18 deployment](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/31a2506f-7eec-482f-9e71-a4d97ae74040)


![cd workflow-19 service](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/06da3651-d996-4594-b2d8-b23deb9b8a27)

then we need create ingress for external port for hte spring gumbal

![cd workflow-18 ingress](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/471886ca-ef06-4c52-92ee-20aa7c2050c8)


YES it shows up spring gumball GKE version here:

![cd workflow-19](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/70d7c20c-a0cf-4593-a123-150399609e5a)


fullscreen

![full screen](https://github.com/mujunyu520/spring-gumball-cicd/assets/60667298/a38692f9-0709-4417-af76-98ba084626ed)

endhere

