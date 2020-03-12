Compilation Environment: Visual Studio 2019

◾ bool CSphere::hasIntersected(CSphere& ball) { } 
두 공이 충돌했는지를 알아보는 함수이다.
두 공 사이의 거리를 반지름의 길이를 두 배한 것보다 작거나 같을 경우 true를 반환, 아니면 false를 반환한다.

◾ void CSphere::hitBy(CSphere& ball) { } 
두 공이 충돌한 경우 충돌 이후 두 공의 속도를 설정해주는 함수이다.
hasIntersected의 리턴값이 true일 경우에 벡터 계산을 통해 충돌 후 두 공의 상태를 설정해준다.

◾ bool CWall::hasIntersected(CSphere& ball) { } 
공이 벽에 충돌했는지를 알아보는 함수이다.
공의 중심좌표가 당구대 범위를 벗어난 경우에 true, 아니면 false를 반환한다.

◾ void CWall::hitBy(CSphere& ball) { } 
공이 벽에 충돌한 후에 공의 상태를 설정해주는 함수이다.
hasIntersected의 리턴값이 true일 경우에 벽에 충돌하는 방향의 속도에 -를 붙여주고 공의 좌표를 벽에서 튕겨나오게 설정해준다.
