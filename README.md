# SWE_2021_41_2024_2_week_6
## week 4 Assignment
* https://github.com/ParkHyungkeun/SWE_2021_41_2024_2_week_4.git 
```python
def isHappy(n):
    list=[]
    while(1):
        list.append(n)
        arr = [int(x) for x in str(n)]
        changed=0
        for x in arr:
            changed+=x**2
        n=changed
        if changed==1:
            return True
        if n in list:
            return False
numb=int(input())
ans=isHappy(numb)
print(ans)
```
* 먼저 정수형 변수를 입력값으로 받는 isHappy라는 함수를 생성한다. \
그 다음 비어있는 리스트를 생성한다.\
그리고, 각 자리수의 제곱의 합을 저장하는 changed 변수를 생성하고, 생성된 changed값을 리스트에 저장한다.\
만약 changed의 값이 1이 되는 순간이 발생하면 True를 반환하고 반복문을 탈출하며, 1이 되지 않은채, 리스트에 있는 숫자와 같은 값이 되는 순간이 발생하면 False를 반환하고 반복문을 탈출한다.\
최종적으로, 정의된 isHappy 함수에 특정 값을 대입하고 그 결과를 출력한다.
## Week 5 Assignment
#### docker exec gallant_euclid cat /etc/os-release
* 이 명령어는 'gallant_euclid'라는 컨테이너 안에서 파일을 출력하는 역할을 합니다. 실행 결과는 PRETTY_NAME="Ubuntu 24.04.1 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04.1 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo로 Ubuntu 버전 및 관련 정보가 출력됩니다.

#### docker exec gallant_euclid git --version
* 이 명령어는 컨테이너 내부에서 설치된 Git의 버전을 확인하는 명령어입니다. 결과로 'git version 2.43.0'과 같은 Git버전이 출력됩니다.

#### docker exec gallant_euclid python3 --version
* 이 명령어는 컨테이너 내부에 설치된 Python3의 버전을 확인하는 명령어입니다. 결과로 'Python 3.12.3'과 같은 Python의 버전이 출력됩니다.

#### docker inspect --format="{{ .HostConfig.Binds }}" gallant_euclid
* 이 명령어는 컨테이너의 바인딩 설정을 출력합니다. 출력 결과는  C:\Users\njjjj\Desktop\opensource:/app와 같이 나타납니다.

