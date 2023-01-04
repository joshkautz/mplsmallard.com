![MPLS Mallard Banner](/Assets/banner.jpg "MPLS Mallard Banner") <!-- 1280 x 640 -->

# MPLS Mallard 🦆

![Production GitHub Workflow Status](https://github.com/joshkautz/subzeroultimate.com/actions/workflows/firebase-hosting-merge.yml/badge.svg "Production GitHub Workflow Status")

## Development 💻

To begin development on the Site, open `./Site/index.html` in your IDE and browser and begin development.

## Deployment 📦

### Automatic: Deploy Site to Firebase Hosting Preview Channel

1. Create a Pull Request to merge a new feature branch into the Main branch.
2. Firebase Hosting GitHub Action will deploy the new changes to a Preview Channel on Firebase Hosting.

### Automatic: Deploy Site to Firebase Hosting Live Channel

3. After testing the features at the Preview Channel URL, merge the Pull Request into the Main branch.
4. Firebase Hosting GitHub Action will deploy the new changes to the Live Channel on Firebase Hosting.

### Manual: Deploy Site to Firebase Hosting Preview Channel

Windows

```PowerShell
$Date = Get-Date -Format "dddd-MM-dd-yyyy-HH-mm-ss"
$Channel = "Preview-" + $Date
firebase hosting:channel:deploy $Channel --expires 3d --project sub-zero-ultimate
```

Linux

```Bash
Date=$(date +'%A-%m-%d-%Y-%H-%M-%S')
Channel="Preview-"$Date
firebase hosting:channel:deploy $Channel --expires 3d --project sub-zero-ultimate
```

### Manual: Deploy Site to Firebase Hosting Live Channel

Windows / Linx

```
firebase deploy --only hosting
```

## Assets

| File       | Purpose                                       |
| ---------- | --------------------------------------------- |
| banner.jpg | Image used in the README.                     |
| icon.png   | Image used to generate the web browser icons. |

<hr>

_This static site was created using the "W3.CSS Templates" from [W3 Schoolers](https://www.w3schools.com/w3css/w3css_templates.asp)._