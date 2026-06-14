# dev   
Connect wifi goog

sudo apt install -y curl;   
curl -fsS https://dl.brave.com/install.sh | sh;   
brave-browser &   
Manually pin to sidebar.

On machine already in Brave sync chain:   
Brave > More tools > Sync > View Sync Code   

On new machine:   
Brave > More tools > Sync > I have a Sync Code   

Login to Gmail   
Login to Bitwarden   
Login to ChatGPT   

cd;   
cp ~/.ssh/authorized_keys ~/.ssh/henrik@home   
cp ~/.ssh/authorized_keys ~/.ssh/henrik@home.pub   

gnome-text-editor ~/.ssh/henrik@home.pub ~/.ssh/henrik@home   

Bitwarden > SSH Key > henrik@home > Copy private key > paste into henrik@home   
Bitwarden > SSH Key > henrik@home > Copy public key > paste into henrik@home.pub   

ssh -X gitgoog.local

cat >> ~/.ssh/config <<'EOF'

Host myserver
    HostName gitgoog.local
    User henrik
    IdentityFile ~/.ssh/henrik@home
EOF
---
# nice to have
gnome-disks &   
Manually pin to sidebar.   

