# Install Git if not installed
# https://git-scm.com/downloads

# Initialize repository
cd arc-tales
git init

# Create .gitignore
echo "node_modules/" > .gitignore
echo ".env" >> .gitignore
echo "cache/" >> .gitignore
echo "artifacts/" >> .gitignore

# Add all files
git add .

# Commit
git commit -m "Initial commit - Arc Tales dApp"

# Create GitHub repo (go to github.com/new)
# Then push:
git remote add origin https://github.com/YOUR_USERNAME/arc-tales.git
git branch -M main
git push -u origin main
