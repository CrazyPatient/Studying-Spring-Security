# Studying-Spring-Security
Studying Spring Security 


Connect Github to sts 
  1. make github repository
  2. sts > open perspective -git > clone url github to sts > make local repository
  ** change to login github ID/pw >> ID/token    have to generate token from github website
  
Update project to git
  1. project > team- shareproject > connect to local repository > project team-add to index(ready to commit) > team - commit (write commit message) > commit and push
  ** plz check sts's project icon and local repository and github **
  
Clone github project to sts
  1. clone github project  using URL
  2. local repository > working tree > project folder - Import projects
  
 Clone others github project to my sts
  1. file- import > git > project from git > clone url > url , id/token next next same to connect github to sts
  
  

--------------------------------------------------------------------------------------------------------
AuthenticationManager > ProviderManager > dao cas remote ....
ProviderManager는 AuthenticationProvicer라는 객체를 이용해 처리 아래로 위임
AuthenticationProvidr앞에 remote cas dao 등 붙어서 처리 +  UserDetailsService인터페이스를 구현하면서 사용자의 정보와 권한정보를 처리해서 반환
개발자가 직접 구현하는 부분은 AuthenticationProvider를 구현하는 방식설계와 직접 UserDetailsService를 구혀하는 방식으로 나뉨
초급단계에선 user정도만 구현하지만 복잡한 프로토콜이나 인증구현방식을 구현할 경우에는 AuthenticationProvider인터페이스를 직접 구현해서 처리
