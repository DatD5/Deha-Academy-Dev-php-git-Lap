# Deha-Academy-Dev-php-git-Lap
 1. Tạo projects:
echo "# Deha-Academy-Dev-php-git-Lab" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

touch index.html

git add index.html

git remote add origin https://github.com/DatD5/Deha-Academy-Dev-php-git-Lap.git

git push -u origin main
![Screenshot 2024-12-23 173441](https://github.com/user-attachments/assets/fd1ac74c-497b-4999-836e-42236f9b3692)
2. Tạo nhánh Develop
git checkout -b develop
touch index.html

git add index.html
git commit -m "edit index.html"

git push origin develop
![Screenshot 2024-12-23 174549](https://github.com/user-attachments/assets/690de051-b40c-4921-a1d1-984d3e7a5f70)
3. Tạo nhánh feature
git checkout -b feature/login

touch login.html

vi login.html

vi index.html

git commit -m'edit index.html and create login.html'
git push origin feature/login
![Screenshot 2024-12-23 181000](https://github.com/user-attachments/assets/8bd9b8b2-5b62-466d-94ee-d8ef4a2b7f67)
git checkout -b feature/loout

touch logout.html

vi logout.html

vi index.html

git commit -m'create logout.html and edit index.html'
git push origin feature/logout
![Screenshot 2024-12-23 182414](https://github.com/user-attachments/assets/eb268d9d-b2ef-4ecd-b0c8-ae359c924514)
4. Merge các nhánh feature trên server Github

5. Tái hiện trường hợp conflict
Trong khi merge feature/logout thì gặp CONFLICT
Đã sửa bằng cách chấp nhận 'Accept Both Changes'
![Screenshot 2024-12-23 181829](https://github.com/user-attachments/assets/53723fc3-1750-442f-893b-a44c01ac6b45)
6. Tạo nhánh release
git checkout -b release/v1.1.0

git commit -m'edit index.html and relese/v1.1.0'
git push origin release/v1.1.0
![Screenshot 2024-12-23 182900](https://github.com/user-attachments/assets/389dafe5-7006-43b0-8010-9b22458a0086)
7. Tạo và xử lý Hotfix
git checkout -b hotfix/v1.1.1

vi index.html

git commit -m'edit index.html and hotfix/v1.1.1'

git push origin hotfix/v1.1.1
![Screenshot 2024-12-23 183806](https://github.com/user-attachments/assets/b6564959-84cb-4656-a7b1-32f02cb867a6)
8. Merge Hotfix vào main và develop
git checkout main

git merge hotfix/fix-login-bug

git push



git checkout develop

git merge hotfix/fix-login-bug

git push



