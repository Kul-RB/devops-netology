# devops-netology
First line

# .gitignore in folder terraform
**/.terraform/* - игнорируютсяся папка .terraform и все файлы внутри вне зависимости от ее раположения
*.tfstate - игнорируются файлы с расширением .tfstate
*.tfstate.* - игнорируются файлы имеющие в названиие .tfstate.
crash.log - игнорируется файл crash.log
crash.*.log - игнорируются файлы, которые начинаются на crash. и имеют расширения .log
*.tfvars - игнорируются файлы с расширением .tfvars
*.tfvars.json - игнорируются файлы с расширением .tfvars.json
override.tf - игнорируется файл override.tf
override.tf.json - игнорируется файл  override.tf.json
*_override.tf - игнорируются файлы название которых заканчиваются на _override.tf
*_override.tf.json - игнорируются файлы название которых заканчиваются на _override.tf.json
.terraformrc - игнорируется файл .terraformrc
terraform.rc - игнорируется файл terraform.rc

#Task 3 change file in new branch
Branch fix
