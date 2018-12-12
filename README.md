"# interview-QnA"

기술면접
목표 : 기술면접 자료 공유 -- 좋은회사취직
이력서

깃허브 저장소

bash 는 콘솔 명령어인걸 알게 해줌

#팀장이 최초 프로젝트 생성 시 수행 작업

## 1. 작업폴더 및 파일

```bash
mkdir interview-QnA
cd interview-QnA
echo "# interview-QnA" >> README.md
```
## 2. 로컬저장소

```bash
git init -- .git 이라는 로컬 저장소폴더 생성
```

## 3. 백업

```bash
git add --all -- 백업대상 등록
git status
git commit -m "first commit"
git log -- 커밋을 조회
```

## 4. 원격저장소 등록(연결)

```bash
git remote add origin https://github.com/LifeOff/interview-QnA.git
git remote -v
```

## 5. 로컬 저장소 =업로드=> 원격 저장소

```bash
git push -u origin master
```

## 6. 팀원에게 접근권한을 부여

```
깃헙 접속 >> settings >> collaborators
>> Search by username, full name or mail address
```

#팀장이 프로젝트 중간에 수행하는 작업

## 1. 작업폴더 및 파일

에디터로 수행하는 작업

## 2. 백업

```bash
git add --all >> 백업대상 등록
git commit -m "first commit"

```

## 3. 로컬 저장소 =업로드=> 원격 저장소
등록된 원격 저장소가 하나일 때 간단하게 업로드가 가능하다.

```bash
git push
```

push를 거부하는 경우에 대처방법은 먼저 pull을 수행하고 그 후 push 하는 것이다.

```bash
git pull
git push
```

*******************************************

# 팀원이 최초 수행하는 작업

## 1. 작업폴더 및 파일
이미 팀장이 수행했으므로 팀원은 팀장의 작업 결과물을 가져오면 된다.

가져오는 코드
```bash
mkdir member-git
cd member-git
git clone (URL)

member-git
git clone https://github.com/snvkdnsem/interview-faq
```

# 팀원이 프로젝트 중간에 수행하는 작업

## 1. 작업폴더 및 파일

에디터로 수행하는 작업

## 2. 백업

```bash
git add --all >> 백업대상 등록
git commit -m "first commit"
```

## 3. 로컬 저장소 =업로드=> 원격 저장소
등록된 원격 저장소가 하나일 때 간단하게 업로드가 가능하다.

```bash
git push
```

push를 거부하는 경우에 대처방법은 먼저 pull을 수행하고 그 후 push 하는 것이다.

```bash
git pull
git push
```
