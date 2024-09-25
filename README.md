# Welcome to My GitHub Profile!

Hello there! I'm Kabindra Ranabhat, a full stack software engineer with a passion for web development, software development and end to end product development. Here you'll find a collection of my projects, repositories, and contributions to the open-source community.

## About Me

- 🌍 **Location:** NSW,Sydney,Australia
- 🎓 **Education:** Bachelor's Degree in Information Technology
- 🌱 **Learning:** Full stack software development lifecycle, Docker, jira, nextjs, node
- 💬 **Ask Me About:** Networking, Javascript, React, Css, web development 
- ⚡ **Fun Fact:** I love hiking, snowbording, soccor, photography, Coding and extreme sports
 
## 📈 My GitHub Stats

![Your GitHub Stats](https://github-readme-stats.vercel.app/api?username=kabindrr&show_icons=true&hide_title=true&hide=prs&count_private=true&theme=radical)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=kabindrr&layout=compact&theme=radical)
![GitHub Streak](https://streak-stats.demolab.com/?user=kabindrr&theme=radical)





## 🛠️ Technologies & Tools



Here are some of the technologies and tools I am familiar with:

### Frontend

![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat&logo=react&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=c-sharp&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=flat&logo=bootstrap&logoColor=white)



### Backend

![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)

### Database

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)


### Tools

![Git](https://img.shields.io/badge/-Git-F05032?style=flat&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Ekahau](https://img.shields.io/badge/Ekahau-FF6F00?style=flat&logo=wifi&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-000000?style=flat&logo=wireshark&logoColor=white)




## 🚀 Projects


Feel free to explore my repositories for more projects and contributions!

## 📫 Get In Touch


- **LinkedIn
:** www.linkedin.com/in/kabindra-ranabhat-31845a92
- **Email:** emailforkabi@gmail.com

## 🤝 How to Contribute
I’m always open to collaboration and contributions. If you’d like to contribute to one of my projects or have an idea for a new one, please check out the contribution guidelines in the respective repositories.

Thank you for visiting my profile! Feel free to drop me a message if you have any questions or just want to connect. Happy coding!
import random

# Sample commit history (you can replace these with real commit messages)
commit_history = [
    "Initial commit",
    "Added README",
    "Fixed bug in function",
    "Updated documentation",
    "Implemented feature X",
    "Refactored code",
    "Optimized performance",
    "Added tests",
    "Fixed typo",
    "Merged branch",
    "Removed deprecated function",
]

# Represent the maze with a simple grid
maze = [
    [' ', ' ', ' ', 'C', ' '],
    [' ', 'G', ' ', ' ', ' '],
    ['C', ' ', 'C', ' ', 'C'],
    [' ', ' ', ' ', 'G', ' '],
    [' ', 'C', ' ', ' ', ' '],
]

# Directions for movement
directions = {
    'w': (-1, 0),  # Up
    's': (1, 0),   # Down
    'a': (0, -1),  # Left
    'd': (0, 1)    # Right
}

def display_maze(player_pos, score):
    for y in range(len(maze)):
        for x in range(len(maze[y])):
            if (y, x) == player_pos:
                print('P', end=' ')
            else:
                print(maze[y][x], end=' ')
        print()
    print(f"Score: {score}\n")

def play_game():
    player_pos = (0, 0)  # Starting position
    score = 0

    while True:
        display_maze(player_pos, score)
        
        move = input("Move (w/a/s/d) or 'q' to quit: ").lower()
        if move == 'q':
            break
        
        if move in directions:
            new_y = player_pos[0] + directions[move][0]
            new_x = player_pos[1] + directions[move][1]
            
            # Check for boundaries
            if 0 <= new_y < len(maze) and 0 <= new_x < len(maze[0]):
                if maze[new_y][new_x] == ' ':
                    player_pos = (new_y, new_x)  # Valid move
                elif maze[new_y][new_x] == 'C':
                    player_pos = (new_y, new_x)
                    score += 1  # Collect commit
                    print("Collected a commit!")
                elif maze[new_y][new_x] == 'G':
                    print("You were caught by a ghost! Game Over.")
                    break
            else:
                print("Invalid move, hit a wall!")
        else:
            print("Invalid input, use w/a/s/d.")

    print("Final Score:", score)

play_game()


---



<!--
**kabindrr/kabindrr** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on Full Stack developer/engineer journey
- 🌱 I’m currently learning docker/view/nextjs/
- 👯 I’m looking to collaborate on fullstack Ecommerce projects
- 🤔 I’m looking for help with ...
- 💬 Ask me about react/node/javascript/
- 📫 How to reach me: emailforkabi@gmail.com
- 😄 Pronouns: 
- ⚡ Fun fact: ...
-->
