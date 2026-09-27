ROLL20 HTML SESSION FILES

Roll20에서 저장/내보낸 HTML 파일을 이 폴더에 넣습니다.

예:
sessions/session-12.html
sessions/session-11.html

그 다음 루트 index.html의 SESSION_HTML_FILES에서 연결합니다.

const SESSION_HTML_FILES={
  "12":"./sessions/session-12.html",
  "11":"./sessions/session-11.html"
};

주의:
- HTML이 이미지/CSS/JS 파일을 별도로 참조한다면 그 파일들도 상대경로를 유지해서 함께 업로드해야 합니다.
- GitHub Pages에서는 정적 HTML 로그를 그대로 표시할 수 있습니다.
- 향후 STUDIO에서 영구 업로드까지 하려면 GitHub Pages만으로는 저장이 안 되므로 서버/스토리지 연결이 필요합니다.
