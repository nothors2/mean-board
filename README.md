## 헤로쿠인터넷 올리기 참조
[단편강좌: Node.js 사이트 Heroku(헤로쿠)로 인터넷에 올리기 - A MEAN Blog](단편강좌: Node.js 사이트 Heroku(헤로쿠)로 인터넷에 올리기 - A MEAN Blog)참조
### 간단정리
package.json => "scripts": {
    "start": "node index.js", 추가
var port = process.env.PORT || 3000;

heroku login
heroku create jamenada-mean-board

git push heroku master

### 확인 : 
[https://jamenada-mean-board.herokuapp.com](https://jamenada-mean-board.herokuapp.com)

### 에러 체크 
heroku logs --tail
### 재시작
heroku start / stop / restart

## 대쉬보드
[https://dashboard.heroku.com/apps](https://dashboard.heroku.com/apps)

###환경변수
heroku config:set MONGO_DB=mongodb+srv://<user>:<pass>@cluster0.x4emn.mongodb.net/board?retryWrites=true&w=majority



## 기존 리포지토리 remote 제거
git remote remove origin

## 새로 연결
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/nothors2/mean-board.git
git push -u origin master
