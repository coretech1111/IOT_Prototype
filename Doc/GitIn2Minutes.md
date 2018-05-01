# 1. Install Git (dùng bản mới nhất)
https://gist.github.com/derhuerst/1b15ff4652a867391f03
# 2. Clone repo từ Git về máy 
## 2.1 Vào thư mục làm việc máy
cd [path to your directory]
## 2.2 Clone project từ github về máy
Command:  $git-clone [Project URLS]

Example: git -clone https://github.com/coretech1111/IOT_Prototype.git

# 3.  Add modified, new file to stage
Command:  $ git  add . 
# 4. Check status for files
Command:           $git status
# 5. Commit files: 
Command:  $ git commit -a -m  "comment" 
 Example: $ git commit -a -m  "Sync 31_3: Correct ADC handling to fix ESP issue, add new ECUmanager module"

# 6. Commit lên git sever
Command: $ git push -[Project URLS]
 Example:
 git -push https://github.com/coretech1111/IOT_Prototype.git