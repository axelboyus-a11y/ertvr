RTN Chat Final - Name + Password Login
=====================================

এই version-এ Gmail/email input নেই।
User login/register: শুধু Name/username + Password।
Admin login: শুধু Admin Password।

IMPORTANT:
1) Supabase Dashboard -> SQL Editor -> New Query এ SUPABASE_REAL_SETUP.sql পুরোটা paste করে Run করতে হবে।
2) Supabase Dashboard -> Authentication -> Providers -> Email -> Confirm email OFF করে দাও।
   কারণ আমরা real Gmail নিচ্ছি না; code ভিতরে username থেকে fake email বানায় যেমন ratan@rtnchat.app।
3) file:// double click না করে START_RTN_CHAT.bat দিয়ে http://localhost:8080 থেকে open করো।

Run:
- START_RTN_CHAT.bat double click
- User app:  http://localhost:8080/user-app.html
- Admin:     http://localhost:8080/admin-panel.html

User create example:
Name/username: ratan
Password: 123456

Admin:
Password: 2026

Feature:
- Name/password account create/login
- Profile photo, cover, bio, note
- Post/story/photo upload
- Like/comment real Supabase database
- Friend request send/accept/reject
- Accept notification
- Messenger-style chat
- Sent/delivered/read status
- Friend হলে photo/file send
- Non-friend হলে শুধু text message
- Blue badge apply
- Admin approve/reject blue badge
- Admin ban/unban, post/story delete, report resolve
- Admin private chat দেখবে না
- Basic WebRTC audio/video call

Note:
HTML-only password admin fully secure না। Real public launch-এর আগে backend/server-side admin auth add করা best। এই version local/testing এবং first MVP setup-এর জন্য।
