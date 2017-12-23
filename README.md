# S3 deploy with CircleCI Example

## Step 1. Setting AWS Key & Secret

CircleCI > Project Settings > Environment > Add Variable

![image](https://user-images.githubusercontent.com/1800369/34319725-79947ab0-e82c-11e7-8754-2423fd688b3b.png)

Add 2 variables `AWS_ACCESS_KEY_ID` `AWS_SECRET_ACCESS_KEY`

![image](https://user-images.githubusercontent.com/1800369/34319724-77c6de94-e82c-11e7-9d6c-abfb3d5ae793.png)


## Step 2. Replace S3 bucket endpoint

Replace `example.com` to `yourbucket.com` on .circleci/config.yml

## How to deploy


|branch| deploy env |
|---|---| 
| develop | **develop** |
| master |  **staging** |
| production | **production** |

