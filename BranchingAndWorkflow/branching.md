# Branching Strategy, Pullrequests, codereview.

#### A branching strategy is a strategy used by development teams to use Git effectively to write, merge and deploy code.Different branching strategies are:
#### 1. GitFlow workflow
#### 2. GitLab workflow
#### 3. GitHub workflow
#### 4. Truck based development

### GitFlow workflow
- Enables parallel development
- Feature branch is created from develop branch. After the completion of changes, feature branch is merged back to develop and master branch.
- Types of branches that can be present are
    - __Master__ branch for production
    - __Develop__ branch for ongoing development
    - __Feature__ branch for new feature
    - __Hotfix__ branch for critical bug fix, branched off from master branch
    - __Release__ branch
- Complex as number of branches increase.
- Increase in chances of merge conflicts.

![Screenshot 2024-12-24 094255](https://github.com/user-attachments/assets/4875afda-c406-4138-96b4-21255e29aa9d)
![Screenshot 2024-12-24 094653](https://github.com/user-attachments/assets/b279f20c-8240-4afd-b24c-c527741182fe)
![Screenshot 2024-12-24 095228](https://github.com/user-attachments/assets/ca2cdb6c-93f7-4bdb-96a6-96a8906924d8)
![Screenshot 2024-12-24 095320](https://github.com/user-attachments/assets/673353e7-c703-4854-9385-f3a8454645fd)
![Screenshot 2024-12-24 095645](https://github.com/user-attachments/assets/c9f39b60-c8ed-4cd8-b7ed-f6fdd0be1055)
![Screenshot 2024-12-24 095755](https://github.com/user-attachments/assets/caede3c4-7ac5-444f-9104-76d3afece0f3)
![Screenshot 2024-12-24 100301](https://github.com/user-attachments/assets/b829ab82-8765-4efa-9437-2c84e3b18aa7)
![Screenshot 2024-12-24 100308](https://github.com/user-attachments/assets/ba48de2f-da67-43fd-be8c-387d29b35073)
![Screenshot 2024-12-24 100325](https://github.com/user-attachments/assets/41b996da-f6ef-4bf3-ac77-efbc701194ab)
![Screenshot 2024-12-24 100333](https://github.com/user-attachments/assets/ea535525-1567-4c55-9702-e210a4bfeade)
![Screenshot 2024-12-24 100357](https://github.com/user-attachments/assets/0f215e8b-6418-444d-b14b-6905ae4fc94d)
![Screenshot 2024-12-24 100451](https://github.com/user-attachments/assets/3160acd7-e427-4d7c-a6b8-0285df1b1280)
![Screenshot 2024-12-24 100953](https://github.com/user-attachments/assets/5f7f183c-4c3b-41f4-a8b9-985519730daf)
![Screenshot 2024-12-24 101026](https://github.com/user-attachments/assets/5254eb43-91f1-49c3-861a-29da9ce9db17)
![Screenshot 2024-12-24 101116](https://github.com/user-attachments/assets/91d496c3-3694-439e-a99e-bfdf66592f0f)
![Screenshot 2024-12-24 101135](https://github.com/user-attachments/assets/f790710c-9fdd-4d05-a738-e215df062149)

### GitLab workflow

- A simpler alternative to GitFlow.
- All fixes and features go to master branch.
- default branch is master.
  
![Screenshot 2024-12-24 104207](https://github.com/user-attachments/assets/57e570ac-30e0-4eca-be2e-6d8d5a050af5)
![Screenshot 2024-12-24 104218](https://github.com/user-attachments/assets/d359ef67-0582-4261-851e-b91813aebd1c)
![Screenshot 2024-12-24 104302](https://github.com/user-attachments/assets/786f2784-7c48-44fc-8875-f1ff2af8d73e)
![Screenshot 2024-12-24 104441](https://github.com/user-attachments/assets/c05dd1ff-d219-433c-a25c-672ae90c07fb)
![Screenshot 2024-12-24 104645](https://github.com/user-attachments/assets/0000b0f5-8f29-4e0e-8f70-a9994ff6991c)
![Screenshot 2024-12-24 104704](https://github.com/user-attachments/assets/408d61ed-ef41-4db8-8017-fcbd9f989d2b)

### GitHub workflow
- no release branches
- only feature branches, which are merged back to master branch.

### Trunk based development

- developers merge small, frequent updates to a core “trunk” or main branch.
