/ git khi làm project cá nhân 

Đẩy code:
git init
git add .
git commit -m "Initial commit"
git remote add origin <URL_repository_của_bạn>
git push -u origin main

update: 
git add .
git commit -m "Update code"
git push -u origin main


// git khi làm việc team work
1. Clone project về 
git clone (url project)
2. sau khi clone tạo một nhánh mới 
git checkout -b (tên nhánh của bạn) main
từ khóa 'main' ở đây có nghĩa là copy những nội dung có trong nhánh chính là main sang nhánh bạn vừa tạo
sau đó thực hiện làm việc trên nhánh đó

mỗi khi bạn code xong thì thực hiện việc push code lên nhưng chú ý thay vì đẩy lên nhánh chính thì bạn phải đẩy lên nhánh bạn vừa tạo
để biết mình đang ở nhánh nào sử dụng lệnh

git branch
và các thao tác 
git add .
git commit -m "message"
git push --set-upstream origin (nhánh của bạn)

//các tình huống thường gặp
khi thành viên code xong thì làm sao để hợp với code chính ở nhánh main ?
- truy cập vào github sau đó tìm tới  Pull Request gửi tới yêu cầu muốn merge code
khi leader duyệt thì code sẽ được update vào nhánh main 
và lúc này bạn  thực hiện việc git checkout -b (tên nhánh của bạn) để truy cập vào nhánh của mình sau đó thực hiện 
git pull origin main

để cập nhật lại code của team update mới nhất
