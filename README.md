# Docker Swarm

### 스웜 초기화

### 노드 추가

### 작업자 노드 사용안함
- 관리자 노드에서 Container 사용시 부하 발생 가능성이 존재하므로 관리자 노드는 관리자 기능으로만 사용
```
docker node update --availability drain <NODE>
```

### 서비스 추가
