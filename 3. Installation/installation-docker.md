# Installation de Docker (Ubuntu/Debian)

## 1. Mettre à jour les paquets :

```zsh
sudo apt update
sudo apt upgrade -y
```

## 2. Installer les dépendances nécessaires :

```zsh
sudo apt install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release -y
```

## 3. Ajouter la clé GPG officielle de Docker :

```zsh
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | \
sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
```

## 4. Ajouter le dépôt Docker à APT :

```zsh
echo \
  "deb [arch=$(dpkg --print-architecture) \
  signed-by=/etc/apt/keyrings/docker.gpg] \
  https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

## 5. Mettre à jour APT et installer Docker Engine :

```zsh
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```

## 6. Verifier que Docker fonctionne :

```zsh
sudo docker version
sudo docker run hello-world
```

**Si une erreur survient, c'est souvent que xia à été mis dans le fichier du dépôt du Docker à la place de noble**

## Etapes pour résoudre l'erreur :

### 1. Editer le fichier du dépôt Docker :

```zsh
sudo nano /etc/apt/sources.list.d/docker.list
```

### 2. Remplacez **xia** par **noble**

**Avant** : `deb [arch=amd64 signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu xia stable`
<br>

**Après** : `deb [arch=amd64 signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu noble stable`

Enregistrez et quittez.

### 3. Ensuite, mettez à jour et réinstallez :

```zsh
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```
