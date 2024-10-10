# DockerTrain1

# Docker installation

## 1.Update Packages
sudo apt update
sudo apt upgrade -y

## 2.Install Dependencies
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y

## 3. Add Docker's GPG Key
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

## 4. Add Docker Repository
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

## 5. Install Docker
sudo apt update
sudo apt install docker-ce -y

## 6. Verify Installation
sudo systemctl status docker

## 7. Run Docker Without Sudo (Optional)
sudo usermod -aG docker $USER

## 8. Test Docker
docker run hello-world

## 9. Install Docker Compose (Optional)
sudo apt install docker-compose -y
