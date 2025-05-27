# 1. Install Git
sudo apt update && sudo apt install git -y        # Ubuntu/Debian
# sudo yum update && sudo yum install git -y      # Amazon Linux/CentOS

# 2. Set Git identity
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# 3. Create a project (or navigate to existing one)
mkdir my-project && cd my-project
touch index.html

# 4. Initialize Git
git init

# 5. Add GitHub repo as remote
git remote add origin https://github.com/your-username/your-repo.git
# or use SSH:
# git remote add origin git@github.com:your-username/your-repo.git

# 6. Stage files for commit
git add .

# 7. (Optional) Check staged changes
git diff --staged

# 8. Commit changes
git commit -m "Initial commit from AWS EC2"

# 9. Push to GitHub
git push -u origin main
# (or master if that's your default branch)
