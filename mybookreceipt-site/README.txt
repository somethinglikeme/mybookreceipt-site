독서 영수증 기록 - 배포 안내

[이미 적용된 것]
- 도메인: https://mybookreceipt.online
- 문의 이메일: goodluck229@gmail.com

[먼저 확인]
압축을 풀고 index.html 을 더블클릭하면 브라우저에서 바로 열립니다 (메뉴 이동 포함).

[GitHub에 올리기]
1. GitHub에서 New repository 로 저장소 생성
2. Add file > Upload files 로 이 폴더 "안의" 파일과 폴더들을 끌어다 놓고 Commit changes
   (저장소 첫 화면에 index.html 이 바로 보여야 합니다)

[Cloudflare Pages 배포]
1. Cloudflare > Workers & Pages > Create application > Pages > Connect to Git
2. GitHub 저장소 선택, Build command 와 Build output directory 는 비워 둠 > Save and Deploy
3. xxx.pages.dev 주소로 열리는지 확인 (메뉴 이동, 영수증 생성, 이미지 저장 테스트)

[도메인 연결]
1. Cloudflare 에서 Add a site 로 mybookreceipt.online 추가 (Free 플랜)
2. Namecheap > Domain List > Manage > Nameservers > Custom DNS 에 Cloudflare 네임서버 2개 입력 후 저장
3. Cloudflare 에서 도메인이 Active 가 되면 Pages 프로젝트 > Custom domains 에서 루트 도메인과 www 를 추가
   (DNS 메뉴에서 CNAME 을 직접 만들지 마세요)

[배포 후]
1. 구글 서치 콘솔 등록 후 https://mybookreceipt.online/sitemap.xml 제출
2. 애드센스 승인 후: 각 HTML <head> 의 ADSENSE 주석 자리에 스크립트 삽입, ads.txt 의 pub-ID 교체,
   광고 슬롯(홈 1곳, 글 하단)을 광고 코드로 교체
