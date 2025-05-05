<!-- ULTRA-PREMIUM ANIMATED HEADER WITH CUSTOM DESIGN -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=300&section=header&text=Nikhil%20Dev%20Arepu&fontAlignY=35&desc=Backend%20Engineer%20|%20Java%20|%20Spring%20Boot%20|%20AWS&descAlignY=55&animation=twinkling&customColorList=0,2,3,1,30" width="100%"/>
</div>
<!-- DYNAMIC TYPING INTRO WITH ENHANCED ANIMATION -->
<p align="center">
  <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&duration=3000&pause=1000&center=true&width=1080&height=100&color=3C99F7&lines=Building+Scalable+Microservices+Architecture;Transforming+Ideas+into+High-Performance+Systems;Let's+Engineer+The+Future+Together!" alt="Typing SVG" /></a>
</p>
<!-- PROFILE VISITOR COUNTER AND SOCIAL BADGES -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Nikhildev0904&style=for-the-badge&color=brightgreen&label=PROFILE+VIEWS" alt="Profile views" />
  <a href="mailto:arrnikhil@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://www.linkedin.com/in/nikhil-dev-arepu">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://leetcode.com/arrnikhil">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=LeetCode&logoColor=black"/>
  </a>
  <a href="https://github.com/Nikhildev0904">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</div>
<!-- INTERACTIVE 3D CONTRIBUTION GRAPH WITH CUSTOM THEME -->
<div align="center">
  <h2>⚙️ GitHub Contribution Skyline</h2>
  <a href="https://skyline.github.com/Nikhildev0904/2023">
    <img src="https://github.com/Nikhildev0904/Nikhildev0904/blob/main/profile-3d-contrib/profile-night-rainbow.svg" width="100%"/>
  </a>
  <i>Click to view my interactive 3D contribution skyline!</i>
</div>
<!-- ANIMATED TECH STACK SHOWCASE -->
<h1 align="center">
  <img src="https://media2.giphy.com/media/QssGEmpkyEOhBCb7e1/giphy.gif?cid=ecf05e47a0n3gi1bfqntqmob8g9aid1oyj2wr3ds3mg700bl&rid=giphy.gif" width="30"> 
  My Tech Arsenal
</h1>
<div align="center">
  <!-- ANIMATED TECH ICONS -->
  <img src="https://user-images.githubusercontent.com/74038190/212257467-871d32b7-e401-42e8-a166-fcfd7baa4c6b.gif" width="100">
  <img src="https://user-images.githubusercontent.com/74038190/212257460-738ff738-247f-4445-a718-cdd0ca76e2db.gif" width="100">
  <img src="https://user-images.githubusercontent.com/74038190/212257454-16e3712e-945a-4ca2-b238-408ad0bf87e6.gif" width="100">
  <img src="https://user-images.githubusercontent.com/74038190/212257468-1e9a91f1-b626-4baa-b15d-5c385dfa7ed2.gif" width="100">
  <img src="https://user-images.githubusercontent.com/74038190/212257465-7ce8d493-cac5-494e-982a-5a9deb852c4b.gif" width="100">
  <img src="https://user-images.githubusercontent.com/74038190/212257463-4d082cb4-ebd7-4532-b550-2db503e63ccb.gif" width="100">
</div>
<!-- INTERACTIVE CODE SNIPPET SHOWCASE -->
<details>
  <summary><h2>💻 Code Sample: My Java Coding Style</h2></summary>
java/**
 * A Sample Spring Boot Service demonstrating my coding style and patterns
 * @author Nikhil Dev Arepu
 */
@Service
@RequiredArgsConstructor
public class UserService {
    private final UserRepository userRepository;
    private final PasswordEncoder passwordEncoder;
    private final JwtTokenProvider tokenProvider;
    
    /**
     * Authenticates a user and returns JWT token
     * Demonstrates error handling patterns and security practices
     */
    public AuthResponse authenticate(LoginRequest request) {
        return userRepository.findByEmail(request.getEmail())
            .filter(user -> passwordEncoder.matches(request.getPassword(), user.getPassword()))
            .map(user -> {
                String token = tokenProvider.generateToken(user);
                return new AuthResponse(token, user.getName());
            })
            .orElseThrow(() -> new AuthenticationException("Invalid credentials"));
    }
    
    /**
     * Creates a new user with validation
     * Shows functional programming style with Java streams
     */
    public User createUser(UserRequest userRequest) {
        // Validate email uniqueness
        if (userRepository.existsByEmail(userRequest.getEmail())) {
            throw new EmailAlreadyExistsException("Email already registered");
        }
        
        // Map DTO to entity using builder pattern
        User newUser = User.builder()
            .name(userRequest.getName())
            .email(userRequest.getEmail())
            .password(passwordEncoder.encode(userRequest.getPassword()))
            .roles(Set.of(Role.USER))
            .createdAt(LocalDateTime.now())
            .build();
            
        return userRepository.save(newUser);
    }
}
</details>
<!-- ABOUT ME SECTION WITH DUAL VIEW -->
<h1 align="center">👨‍💻 About Me</h1>
<table>
  <tr>
    <td width="50%">
      <h3>Professional Identity</h3>
      <p>
        As a <b>Backend Engineer</b> passionate about crafting scalable solutions, I specialize in building high-performance distributed systems using <b>Java</b>, <b>Spring Boot</b>, and <b>AWS</b>. My expertise is focused on creating robust microservices architectures that solve complex business problems efficiently.
      </p>
      <p>
        At <b>Cognitree</b>, I've been developing production-grade applications with a focus on performance optimization, security best practices, and clean, maintainable code. My approach combines technical excellence with business-oriented thinking.
      </p>
  <h3>My Engineering Philosophy</h3>
  
  > "Software development is not just about writing code; it's about crafting elegant solutions to real-world problems. Great code should be clean, maintainable, and scalable."
  
  <div align="center">
    <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical&quote=First%20solve%20the%20problem%2C%20then%20write%20the%20code.&author=John%20Johnson" width="100%"/>
  </div>
</td>
<td width="50%">
  <img src="https://github.com/abhisheknaiidu/abhisheknaiidu/blob/master/code.gif?raw=true" width="100%">
  
  <h3>Key Competencies</h3>
  <ul>
    <li>🔹 <b>Backend Development:</b> Java, Spring Boot, Microservices</li>
    <li>🔹 <b>Database Systems:</b> PostgreSQL, MongoDB, MySQL</li>
    <li>🔹 <b>Cloud & DevOps:</b> AWS, Docker, CI/CD</li>
    <li>🔹 <b>Architecture:</b> Microservices, System Design</li>
    <li>🔹 <b>Performance:</b> Optimization, Caching, Scaling</li>
  </ul>
  
  <h3>GitHub Streak</h3>
  <a href="https://git.io/streak-stats">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=Nikhildev0904&theme=dark&hide_border=true&background=0D1117&stroke=3C99F7&ring=3C99F7&fire=FF6347&currStreakNum=3C99F7&sideNums=3C99F7&currStreakLabel=3C99F7&sideLabels=3C99F7&dates=8B949E" width="100%" />
  </a>
</td>
  </tr>
</table>
<!-- INTERACTIVE METRICS DASHBOARD -->
<h1 align="center">📊 Performance Metrics</h1>
<div align="center">
  <!-- GitHub Stats Card with Custom Theme -->
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Nikhildev0904&count_private=true&show_icons=true&theme=react&hide_border=true&bg_color=0D1117&title_color=3C99F7&icon_color=F8D866" />
  <!-- Most Used Languages Card -->
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nikhildev0904&layout=compact&hide_border=true&theme=react&bg_color=0D1117&title_color=3C99F7&langs_count=8&exclude_repo=oldRepos" />
  <!-- GitHub Trophies with Custom Theme -->
  <img width="800em" src="https://github-profile-trophy.vercel.app/?username=Nikhildev0904&theme=algolia&column=8&margin-w=15&margin-h=15&no-frame=true&rank=SSS,SS,S,AAA,AA,A,B,C" />
  <!-- Activity Graph -->
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph/?username=Nikhildev0904&theme=react-dark&hide_border=true&area=true" />
</div>
<!-- TOGGLE BETWEEN DARK/LIGHT THEME CONTENT (GITHUB SPECIAL SYNTAX) -->
<div align="center">
  <h2>🌓 Viewing Experience</h2>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nikhildev0904/Nikhildev0904/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nikhildev0904/Nikhildev0904/output/github-contribution-grid-snake.svg">
    <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/Nikhildev0904/Nikhildev0904/output/github-contribution-grid-snake.svg">
  </picture>
  <p><i>The snake animation adapts to your theme preference! Try switching between light/dark mode.</i></p>
</div>
<!-- SKILL SHOWCASE WITH ADVANCED VISUALS -->
<h1 align="center">🛠️ Technical Expertise</h1>
<!-- PREMIUM SKILL VISUALIZATION -->
<div align="center">
  <table>
    <tr>
      <td>
        <img src="https://img.shields.io/badge/-%20Backend%20Technology%20Stack-1A1B27?style=for-the-badge&labelColor=222&color=1A1B27" />
        <br><br>
        <div>
          <img src="https://techstack-generator.vercel.app/java-icon.svg" alt="Java" width="65" height="65" />
          <img src="https://skillicons.dev/icons?i=spring" width="65" height="65" alt="Spring" />
          <img src="https://skillicons.dev/icons?i=hibernate" width="65" height="65" alt="Hibernate" />
          <img src="https://skillicons.dev/icons?i=maven" width="65" height="65" alt="Maven" />
        </div>
        <br>
        <div style="margin-bottom: 5px;">
          <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00.svg?style=flat&logo=java&logoColor=white"/>
          <img alt="Spring" src="https://img.shields.io/badge/Spring-6DB33F.svg?style=flat&logo=spring&logoColor=white"/>
          <img alt="Hibernate" src="https://img.shields.io/badge/Hibernate-59666C.svg?style=flat&logo=hibernate&logoColor=white"/>
          <img alt="JUnit" src="https://img.shields.io/badge/JUnit5-25A162.svg?style=flat&logo=check-circle&logoColor=white"/>
        </div>
        <br>
        <img src="https://progress-bar.dev/95/?width=500&scale=100&title=Java&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/90/?width=500&scale=100&title=Spring%20Boot&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/85/?width=500&scale=100&title=Hibernate&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/80/?width=500&scale=100&title=JUnit&suffix=&color=3C99F7" />
      </td>
      <td>
        <img src="https://img.shields.io/badge/-%20Cloud%20%26%20DevOps-1A1B27?style=for-the-badge&labelColor=222&color=1A1B27" />
        <br><br>
        <div>
          <img src="https://techstack-generator.vercel.app/aws-icon.svg" alt="AWS" width="65" height="65" />
          <img src="https://techstack-generator.vercel.app/docker-icon.svg" alt="Docker" width="65" height="65" />
          <img src="https://skillicons.dev/icons?i=kubernetes" width="65" height="65" alt="Kubernetes" />
          <img src="https://skillicons.dev/icons?i=githubactions" width="65" height="65" alt="GitHub Actions" />
        </div>
        <br>
        <div style="margin-bottom: 5px;">
          <img alt="AWS" src="https://img.shields.io/badge/AWS-FF9900.svg?style=flat&logo=amazon-aws&logoColor=white"/>
          <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=docker&logoColor=white"/>
          <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5.svg?style=flat&logo=kubernetes&logoColor=white"/>
          <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-2088FF.svg?style=flat&logo=github-actions&logoColor=white"/>
        </div>
        <br>
        <img src="https://progress-bar.dev/85/?width=500&scale=100&title=AWS&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/80/?width=500&scale=100&title=Docker&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/65/?width=500&scale=100&title=Kubernetes&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/75/?width=500&scale=100&title=CI/CD&suffix=&color=3C99F7" />
      </td>
    </tr>
    <tr>
      <td>
        <img src="https://img.shields.io/badge/-%20Database%20Systems-1A1B27?style=for-the-badge&labelColor=222&color=1A1B27" />
        <br><br>
        <div>
          <img src="https://techstack-generator.vercel.app/mysql-icon.svg" alt="MySQL" width="65" height="65" />
          <img src="https://skillicons.dev/icons?i=mongodb" width="65" height="65" alt="MongoDB" />
          <img src="https://skillicons.dev/icons?i=postgres" width="65" height="65" alt="PostgreSQL" />
          <img src="https://skillicons.dev/icons?i=redis" width="65" height="65" alt="Redis" />
        </div>
        <br>
        <div style="margin-bottom: 5px;">
          <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1.svg?style=flat&logo=mysql&logoColor=white"/>
          <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-47A248.svg?style=flat&logo=mongodb&logoColor=white"/>
          <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-336791.svg?style=flat&logo=postgresql&logoColor=white"/>
          <img alt="Redis" src="https://img.shields.io/badge/Redis-DC382D.svg?style=flat&logo=redis&logoColor=white"/>
        </div>
        <br>
        <img src="https://progress-bar.dev/90/?width=500&scale=100&title=MySQL&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/85/?width=500&scale=100&title=MongoDB&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/80/?width=500&scale=100&title=PostgreSQL&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/75/?width=500&scale=100&title=Redis&suffix=&color=3C99F7" />
      </td>
      <td>
        <img src="https://img.shields.io/badge/-%20Other%20Technologies-1A1B27?style=for-the-badge&labelColor=222&color=1A1B27" />
        <br><br>
        <div>
          <img src="https://techstack-generator.vercel.app/python-icon.svg" alt="Python" width="65" height="65" />
          <img src="https://techstack-generator.vercel.app/js-icon.svg" alt="JavaScript" width="65" height="65" />
          <img src="https://skillicons.dev/icons?i=react" width="65" height="65" alt="React" />
          <img src="https://skillicons.dev/icons?i=git" width="65" height="65" alt="Git" />
        </div>
        <br>
        <div style="margin-bottom: 5px;">
          <img alt="Python" src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=python&logoColor=white"/>
          <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat&logo=javascript&logoColor=black"/>
          <img alt="React" src="https://img.shields.io/badge/React-61DAFB.svg?style=flat&logo=react&logoColor=black"/>
          <img alt="Git" src="https://img.shields.io/badge/Git-F05032.svg?style=flat&logo=git&logoColor=white"/>
        </div>
        <br>
        <img src="https://progress-bar.dev/75/?width=500&scale=100&title=Python&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/70/?width=500&scale=100&title=JavaScript&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/65/?width=500&scale=100&title=React&suffix=&color=3C99F7" />
        <img src="https://progress-bar.dev/90/?width=500&scale=100&title=Git&suffix=&color=3C99F7" />
      </td>
    </tr>
  </table>
</div>
<!-- ARCHITECTURE & CONCEPTS BADGES WITH TOOLTIPS -->
<div align="center">
  <h3>Architecture & Advanced Concepts</h3>
  <img src="https://img.shields.io/badge/Microservices-FF6C37?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/REST_API-009688?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white" />
  <img src="https://img.shields.io/badge/Design_Patterns-3C873A?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/SOLID_Principles-FF7F00?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/System_Design-6236FF?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Multithreading-0074D9?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Event_Driven-7D3C98?style=for-the-badge&logoColor=white" />
</div>
<!-- FEATURED PROJECTS WITH ARCHITECTURE DIAGRAMS -->
<h1 align="center">🏆 Showcase Projects</h1>
<!-- PROJECT SHOWCASE WITH ARCHITECTURE DIAGRAMS -->
<table>
  <tr>
    <td colspan="2">
      <div align="center">
        <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" />
      </div>
      <h2 align="center">🏥 Smart Healthcare Appointment System</h2>
    </td>
  </tr>
  <tr>
    <td width="60%">
      <img src="https://user-images.githubusercontent.com/74038190/212749171-b84692a8-2b04-4e3b-93ca-ac14705da224.gif" width="100%" alt="Project Overview"/>
    </td>
    <td width="40%">
      <h3>A Microservices-based Healthcare Platform</h3>
      <p>
        Advanced appointment management system built with Spring Boot and React to revolutionize healthcare operations through digital transformation.
      </p>
  <details>
    <summary><b>🔍 View System Architecture</b></summary>
    <div align="center">
      <img src="https://miro.medium.com/v2/resize:fit:1400/1*wTO7Ka0D4grrFEs9pONSmA.png" width="100%" alt="Architecture Diagram"/>
      <i>Microservices architecture with event-driven communication</i>
    </div>
  </details>
  
  <h4>Core Technologies:</h4>
  <div>
    <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white" />
    <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
    <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=json-web-tokens&logoColor=white" />
    <img src="https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socket.io&logoColor=white" />
    <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
  </div>
  
  <h4>Performance Metrics:</h4>
  <ul>
    <li><b>99.5% uptime</b> with high availability configuration</li>
    <li><b>Response times under 200ms</b> even under peak load</li>
    <li><b>500+ daily active users</b> with seamless experience</li>
    <li><b>40% reduction</b> in administrative overhead</li>
    <li><b>30% increase</b> in appointment completion rate</li>
  </ul>
</td>
  </tr>
</table>
<!-- PROJECT 2 -->
<table>
  <tr>
    <td colspan="2">
      <div align="center">
        <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" />
      </div>
      <h2 align="center">🦜 Birdz: Bird Species Classification App</h2>
    </td>
  </tr>
  <tr>
    <td width="40%">
      <h3>AI-powered Mobile Application</h3>
      <p>
        A cutting-edge Flutter application using deep learning models to identify Indian bird species in their natural habitats with remarkable accuracy.
      </p>
  <details>
    <summary><b>🔍 View System Architecture</b></summary>
    <div align="center">
      <img src="https://miro.medium.com/v2/resize:fit:1400/1*Lqf38GJGKzNCxOtHGNZU5g.png" width="100%" alt="Architecture Diagram"/>
      <i>Serverless architecture with AI model integration</i>
    </div>
  </details>
  
  <h4>Technical Stack:</h4>
  <div>
    <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" />
    <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
    <img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
    <img src="https://img.shields.io/badge/REST_API-009688?style=flat-square&logo=fastapi&logoColor=white" />
  </div>
  
  <h4>Advanced Features:</h4>
  <ul>
    <li><b>Dual AI model approach</b> combining ResNet50 and YOLOv8</li>
    <li><b>Custom-built dataset</b> with 6,952 annotated bird images</li>
    <li><b>Offline classification</b> capability for remote use</li>
    <li><b>Bird species encyclopedia</b> with detailed information</li>
    <li><b>Community contribution</b> module for dataset expansion</li>
  </ul>
</td>
<td width="60%">
  <img src="https://user-images.githubusercontent.com/74038190/218265814-3084a4ba-809c-4135-afc0-8685d0f634b3.gif" width="100%" alt="Birdz App"/>
</td>
  </tr>
</table>
<!-- INTERACTIVE DEVELOPMENT JOURNEY ROADMAP -->
<h1 align="center">🗺️ My Software Engineering Journey</h1>
<div align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" />
</div>
<!-- CAREER TIMELINE WITH VISUAL ELEMENTS -->
<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/235224431-e8c8c12e-6826-47f1-89fb-2ddad83b3abf.gif" width="300" />
</div>
<div class="timeline">
  <!-- EXPERIENCE TIMELINE WITH ICONS -->
  <table>
    <tr>
      <td width="15%" align="center">
        <img src="https://img.shields.io/badge/2025-Present-3C99F7?style=for-the-badge" />
        <br><br>
        <img src="https://skillicons.dev/icons?i=spring" width="50" height="50" alt="Spring" />
      </td>
      <td width="85%">
        <div style="border-left: 3px solid #3C99F7; padding-left: 20px; margin-bottom: 20px;">
          <h3>Software Engineer Intern</h3>
          <h4>Cognitree Pvt Ltd</h4>
          <p>Leading microservices development with Spring Boot and deploying with containerization on AWS.</p>
          <ul>
            <li>Designing and implementing APIs following REST best practices</li>
            <li>Optimizing database queries for performance enhancement</li>
            <li>Implementing security measures including JWT authentication</li>
            <li>Creating CI/CD pipelines for automated testing and deployment</li>
          </ul>
        </div>
      </td>
    </tr>
    <tr>
      <td width="15%" align="center">
        <img src="https://img.shields.io/badge/2023-2023-3C99F7?style=for-the-badge" />
        <br><br>
        <img src="https://skillicons.dev/icons?i=react" width="50" height="50" alt="React" />
      </td>
      <td width="85%">
        <div style="border-left: 3px solid #3C99F7; padding-left: 20px; margin-bottom: 20px;">
          <h3>Java Full Stack Developer</h3>
          <h4>iamneo (Formerly Examly)</h4>
          <p>Built full-stack applications with Java backend and React frontend.</p>
          <ul>
            <li>Developed RESTful APIs for data retrieval and manipulation</li>
            <li>Designed responsive UI components with React and Material UI</li>
            <li>Implemented authentication and authorization workflows</li>
            <li>Deployed applications on AWS cloud infrastructure</li>
          </ul>
        </div>
      </td>
    </tr>
    <tr>
      <td width="15%" align="center">
        <img src="https://img.shields.io/badge/2022-2023-3C99F7?style=for-the-badge" />
        <br><br>
        <img src="https://skillicons.dev/icons?i=github" width="50" height="50" alt="GitHub" />
      </td>
      <td width="85%">
        <div style="border-left: 3px solid #3C99F7; padding-left: 20px; margin-bottom: 20px;">
          <h3>Core Team Member</h3>
          <h4>CodeChef VIT-AP Chapter</h4>
          <p>Organized technical events and mentored peers in programming.</p>
          <ul>
            <li>Created problem statements for competitive programming contests</li>
            <li>Conducted workshops on data structures and algorithms</li>
            <li>Mentored junior students in coding and problem-solving</li>
            <li>Built the chapter's technical community and online presence</li>
          </ul>
        </div>
      </td>
    </tr>
  </table>
</div>
<!-- EDUCATION SECTION -->
<h1 align="center">🎓 Education & Learning</h1>
<table>
  <tr>
    <td width="30%">
      <img src="https://user-images.githubusercontent.com/74038190/212748842-9fcbad5b-6173-4175-8a61-521f3dbb7514.gif" width="100%" />
    </td>
    <td width="70%">
      <h3>Vellore Institute of Technology (VIT-AP)</h3>
      <p><b>Bachelor of Technology in Computer Science and Engineering</b></p>
      <p>2021 - 2025 | CGPA: 8.79/10</p>
  <h4>Key Coursework:</h4>
  <div>
    <img src="https://img.shields.io/badge/Data_Structures-007396?style=flat-square" />
    <img src="https://img.shields.io/badge/Algorithms-00599C?style=flat-square" />
    <img src="https://img.shields.io/badge/Operating_Systems-FCC624?style=flat-square" />
    <img src="https://img.shields.io/badge/Database_Management-4479A1?style=flat-square" />
    <img src="https://img.shields.io/badge/Software_Engineering-512BD4?style=flat-square" />
    <img src="https://img.shields.io/badge/Computer_Networks-0078D4?style=flat-square" />
    <img src="https://img.shields.io/badge/Web_Development-E34F26?style=flat-square" />
    <img src="https://img.shields.io/badge/Cloud_Computing-FF9900?style=flat-square" />
  </div>
  
  <h4>Professional Learning Path:</h4>
  <div>
    <img src="https://progress-bar.dev/95/?width=300&scale=100&title=DSA&suffix=&color=3C99F7" />
    <img src="https://progress-bar.dev/90/?width=300&scale=100&title=System%20Design&suffix=&color=3C99F7" />
    <img src="https://progress-bar.dev/85/?width=300&scale=100&title=Cloud%20Native&suffix=&color=3C99F7" />
    <img src="https://progress-bar.dev/80/?width=300&scale=100&title=DevOps&suffix=&color=3C99F7" />
  </div>
</td>
  </tr>
</table>
<!-- CERTIFICATIONS WITH VISUAL BADGES -->
<h1 align="center">🏅 Certifications & Achievements</h1>
<div align="center">
  <a href="#">
    <img src="https://img.shields.io/badge/Oracle_Cloud-Database_Development-FF0000?style=for-the-badge&logo=oracle&logoColor=white" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/iamNeo-Java_Full_Stack_Developer-1E88E5?style=for-the-badge&logo=java&logoColor=white" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/GFG-Top_2%25_University_Leaderboard-2F8D46?style=for-the-badge&logo=geeksforgeeks&logoColor=white" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/DSA-500+_Problems_Solved-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" />
  </a>
</div>
<!-- INTERACTIVE RESOURCES SECTION -->
<h1 align="center">🔗 Resources & Tools I Recommend</h1>
<table>
  <tr>
    <td width="33%">
      <h3 align="center">For Backend Developers</h3>
      <ul>
        <li><a href="https://spring.io/guides">Spring Boot Guides</a></li>
        <li><a href="https://12factor.net/">The Twelve-Factor App</a></li>
        <li><a href="https://microservices.io/patterns/index.html">Microservice Architecture Patterns</a></li>
        <li><a href="https://www.baeldung.com/">Baeldung Java Tutorials</a></li>
        <li><a href="https://docs.aws.amazon.com/index.html">AWS Documentation</a></li>
      </ul>
    </td>
    <td width="33%">
      <h3 align="center">For System Design</h3>
      <ul>
        <li><a href="https://github.com/donnemartin/system-design-primer">System Design Primer</a></li>
        <li><a href="https://www.educative.io/courses/grokking-the-system-design-interview">Grokking System Design</a></li>
        <li><a href="https://martinfowler.com/articles/microservices.html">Microservices by Martin Fowler</a></li>
        <li><a href="https://highscalability.com/">High Scalability Blog</a></li>
        <li><a href="https://www.designgurus.io/">Design Gurus</a></li>
      </ul>
    </td>
    <td width="33%">
      <h3 align="center">For DevOps & Cloud</h3>
      <ul>
        <li><a href="https://www.docker.com/resources/what-container">Docker Resources</a></li>
        <li><a href="https://kubernetes.io/docs/home/">Kubernetes Documentation</a></li>
        <li><a href="https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html">AWS Well-Architected Framework</a></li>
        <li><a href="https://12factor.net/">The Twelve-Factor App</a></li>
        <li><a href="https://roadmap.sh/devops">DevOps Roadmap</a></li>
      </ul>
    </td>
  </tr>
</table>
<!-- GET IN TOUCH SECTION -->
<h1 align="center">📫 Connect With Me</h1>
<div align="center">
  <a href="mailto:arrnikhil@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://www.linkedin.com/in/nikhil-dev-arepu">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://leetcode.com/arrnikhil">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=LeetCode&logoColor=black"/>
  </a>
  <a href="https://github.com/Nikhildev0904">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</div>
<div align="center">
  <h3>✉️ Open for collaboration, project opportunities, and networking!</h3>
  <p>Let's connect and discuss how we can work together on exciting projects.</p>
</div>
<!-- ANIMATED WAVES FOOTER -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=150&section=footer&fontSize=50&fontAlignY=65&animation=twinkling&customColorList=0,2,3,1,30" width="100%"/>
</div>
<div align="center">
  <h2>✨ "Clean code always looks like it was written by someone who cares." ✨</h2>
  <p>Thank you for visiting my profile! Let's build something amazing together.</p>
</div>
<!-- SETUP INSTRUCTIONS FOR GITHUB ACTIONS -->
<!-- 
For the 3D contribution calendar:
1. Create a file at .github/workflows/profile-3d.yml with:

name: GitHub-Profile-3D-Contrib
on:
  schedule:
    - cron: "0 18 * * *"
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v2
      - uses: yoshi389111/github-profile-3d-contrib@0.7.0
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: ${{ github.repository_owner }}
      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          git commit -m "generated"
          git push

For the snake animation:
1. Create a file at .github/workflows/snake.yml with:

name: Generate Snake Animation
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          svg_out_path: dist/github-contribution-grid-snake.svg
          snake_color: 'blue'
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-->
