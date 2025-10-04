# Update Existing GitHub Repository Commands

# 1. Clone your existing repository
git clone https://github.com/shiva63431/lib.git
cd lib

# 2. Copy files from our prepared folder
# Copy README.md
copy "..\vision-libraries-github\README.md" "README.md"

# Copy libs folder
xcopy "..\vision-libraries-github\libs" "libs" /E /I

# 3. Add and commit changes
git add .
git commit -m "Add Vision libraries and comprehensive documentation"

# 4. Push to GitHub
git push origin main

# Alternative: If you want to replace the .rar file
# Delete old file first
git rm arm64-v8a.rar
git commit -m "Remove old .rar file, add organized libraries"
git push origin main
