I. Set up Oh-my-posh
1. Document: https://ohmyposh.dev/docs/
3. Window<br>
   2.1 winget install JanDeDobbeleer.OhMyPosh -s winget (more details on https://ohmyposh.dev/docs/installation/windows)<br>
   2.2 $env:Path += ";\<path to ohMyPosh executive file>"<br>
   2.3 Confirm that oh my posh command works: (Get-Command oh-my-posh).Source<br>
   2.4 Follow https://ohmyposh.dev/docs/installation/prompt to update the prompt.<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.1 Create the file if not existed: New-Item -Path $PROFILE -Type File -Force<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.2 Open the file ```notepad $PROFILE```<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.3 Add ```oh-my-posh init pwsh --config "<link to the template>" | Invoke-Expression to the file```<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.4 Execute the file to apply the prompt format ```. $PROFILE```<br>
   2.5 Follow https://ohmyposh.dev/docs/installation/fonts to update the font<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.1 Install neccessary fonts ```oh-my-posh font install``` and ```oh-my-posh font install meslo```<br>
     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.2 Make sure to update the font on each application such as jetbrains's products, vscode, window terminal<br>
5. MacOS (zsh)<br>
   3.1 ```brew install jandedobbeleer/oh-my-posh/oh-my-posh``` (more details on https://ohmyposh.dev/docs/installation/windows](https://ohmyposh.dev/docs/installation/macos)<br>
   3.2 Open the file responsible for zsh terminal ```vi ~/.zshrc```<br>
   3.3 Add ```eval "$(oh-my-posh init zsh)"``` to .zshrc<br>
   3.4 Follow https://ohmyposh.dev/docs/installation/prompt to update the prompt.<br>
   3.5 Follow https://ohmyposh.dev/docs/installation/fonts to update the font<br>
   
