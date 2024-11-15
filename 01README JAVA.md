
## Prerequisites:
- In your BTP sub account,you have [initially set up you SAP Business Application Studio(BAS)](https://help.sap.com/docs/bas/sap-business-application-studio/getting-started) and created Dev Space in Full Stack Cloud Application.

## Steps:

- Step 1,  Change folder to Projects in BAS

![alt text](image.png)
![alt text](image-1.png)

- Step 2, Clone code from git hub.
Run the following command in BAS terminal:
```bash
git clone https://github.com/horsemanjackyliu/labelprintinginjava.git
```
![alt text](image-79.png)

- Step 3, Build the application with the following command in BAS terminal:
```bash
cd labelprintinginjava
mvn clean install
npm run build
```
![alt text](image-80.png)
![alt text](image-81.png)
![alt text](image-82.png)




- Step 4, login into BTP SubAccount with the following command in BAS terminal:
```bash
cf login -a <cloud foundry api>
```

You can get the cloud foundry API in BTP SubAccount with the following screenshot:
![alt text](image-4.png)
![alt text](image-6.png)

- Step 5, Run the following command in BAS terminal to deploy the application into BTP SubAccount cloud foundry environment .

```bash
npm run deploy
```
![alt text](image-83.png)


- Step 6, Create role collection and assign the role to the end user in BTP SubAccount.

![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)
![alt text](image-11.png)
![alt text](image-12.png)
![alt text](image-13.png)











