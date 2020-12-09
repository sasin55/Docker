# Docker Swarm

### 스웜 초기화

### 노드 추가

### 노드 권한 변경
1. 노드 승격( Manager Node )
```
* 편의를 위한 명령어
  - docker node promote <NODE>
  
* 기본 명령어
  - docker node update --role manager <NODE>
```
2. 노드 강등( Woker Node )
```
* 편의를 위한 명령어
  - docker node demote <NODE>
  
* 기본 명령어
  - docker node update --role worker <NODE>
```

### 노드 삭제
```
docker node rm <NODE>
```

### 작업자 노드 사용안함
- 관리자 노드에서 Container 사용시 부하 발생 가능성이 존재하므로 관리자 노드는 관리자 기능으로만 사용
```
docker node update --availability drain <NODE>
```

### 서비스 추가
