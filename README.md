In this project, a static web site is hosted on a container on ec2.

Sudo apt update
Sudo apt intall docker.io -y
Sudo usermod -aG docker ubuntu
Sudo reboot
ssh -i "mykey.pem" ubuntu@ec2-54-214-76-241.us-west-2.compute.amazonaws.com
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/your-username/your-repo.git
git branch -M main   # Optional: rename current branch to main
git push -u origin main
Sudo apt install git
Git clone https://github.com/itskhanarif/primecare-html.git
 docker build -t primecare-html-images .
docker run -d -p 8080:80 --name primecare-html-container primecare-html-images
add secuirity group rule that custom tcp port 8080 from anywhere IPv4
docker stop container_id
docker rm container_id
docker rmi image_id
sudo rm -r folder_name
