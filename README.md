- 👋 Hi, I’m @TheBhupenderSingh
- 👀 I’m interested in ...learning new techs in web development
- 🌱 I’m currently learning ...  complicated Backend development using springboot and React framework.
- 💞️ I’m looking to collaborate on ... any projects related to Java Springboot backend and React, Node.js Frontend
- 📫 How to reach me ... Email me on lkywww1@gmail.com
- 😄 Pronouns: ...He


<!---
TheBhupenderSingh/TheBhupenderSingh is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


server {
    listen 80;
    server_name myapp.local;

    location / {
        proxy_pass http://127.0.0.1:8080;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
}
