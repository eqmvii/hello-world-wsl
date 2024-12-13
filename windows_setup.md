Open console / command prompt / power shell and run: wsl --install

(latest version is important) 

Open Create new account / pw

example will be "wadmin" as ubuntu user in the wsl 
wadmin 

Commands and steps:

Open pwd in windows explorer: explorer.exe .
Example: \\wsl.localhost\Ubuntu\home\wadmin 

wadmin being my new username 

setup git
git config --global user.name "usernamegoeshere"

SSH: ssh-keygen -t ed25519 -C "email@example.com"
saved to /home/wadmin/.ssh/id_ed25519

Add to SSH agent:
for linux: eval "$(ssh-agent -s)"Agent pid 828
add:
ssh-add ~/.ssh/id_ed25519 
$ cat ~/.ssh/id_ed25519.pub# Then select and copy the contents of the id_ed25519.pub file# displayed in the terminal to your clipboard

paste on GH

then locally test with: 
 ssh -T git@github.com

Hi username! You've successfully authenticated, but GitHub does not provide shell access. 
