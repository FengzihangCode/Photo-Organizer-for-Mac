# Photo Organizer

Photo Organizer是一个适用于Windows/macOS/Linux的脚本，旨在帮助作者自己整理照片文件夹中的照片。它提供了两种整理方式：

1. **按拍摄日期整理：**根据拍摄日期创建文件夹，并将照片移动到相应的日期文件夹中。
2. **按文件格式整理：**根据文件格式（JPG、ARW 等）将照片移动到不同的文件夹中。

## 如何使用（针对Bash）

1. 将 `photo_organizer.sh` 文件复制到包含您照片的文件夹中。
2. 在终端中导航到该文件夹（cd 路径）。
3. 运行以下命令：

```
./photo_organizer.sh
```

4. 根据提示选择整理方式（输入1或2），并按照指示操作即可。

## 注意事项

- 确保放置该脚本的文件夹中包含要整理的照片。
- 脚本支持处理以下常见的照片格式：JPG、ARW、NEF、ORF、RW2、RAF 和 DNG。
- 在移动文件时，脚本会进行错误处理，并在发生错误时显示相应的错误消息。
- 如果需要处理其他格式的文件或指定不同的目录，请参考脚本中的参数化部分，并相应修改。
- 请注意，可能需要给予执行权限 (chmod +x photo_organizer.sh)

## 系统要求

- Linux 发行版（如 Ubuntu、Fedora、Debian 等 P.S. Ubuntu永远的神 ——作者）
- macOS
- Windows

## 常见故障排除

在使用Photo Organizer时，可能会遇到一些常见的错误。以下是一些可能出现的错误以及对应的解决方案：

	1.	找不到照片文件：
	•	错误描述： 运行脚本后，脚本显示 “No photo files found.” 错误消息。
	•	解决方案： 确保您运行脚本的文件夹中包含您要整理的照片文件。如果文件夹中确实有照片文件，但脚本仍然无法找到，请检查文件名是否正确或文件权限是否设置正确。
	2.	创建目录失败：
	•	错误描述： 运行脚本后，脚本显示 “Error: Failed to create directory” 错误消息。
	•	解决方案： 这可能是由于文件系统权限问题导致的。请确保您对目录具有写入权限。您还可以尝试手动创建目录以查看是否存在其他问题。
	3.	移动文件失败：
	•	错误描述： 运行脚本后，脚本显示 “Error: Failed to move file” 错误消息。
	•	解决方案： 这可能是由于文件系统权限问题或文件被其他进程占用导致的。请确保您对目标文件夹具有写入权限，并且文件没有被其他程序锁定。您可以尝试手动移动文件以排除问题。
	4.	输入无效选项：
	•	错误描述： 运行脚本后，脚本显示 “Invalid option. Please select again.” 错误消息。
	•	解决方案： 这可能是因为用户输入了无效的选项。请按照脚本提供的选项进行选择，并确保输入的选项是 1、2 或 3。检查输入是否有误并重新输入正确的选项。
	5.	未安装必要的工具：
	•	错误描述： 运行脚本后，脚本显示类似 “command not found” 的错误消息。
	•	解决方案： 这可能是由于您的系统缺少所需的工具或环境变量配置不正确所致。请确保您的系统上安装了 Bash 和其他所需的 Unix 工具，或者尝试在另一台系统上运行脚本。

## 关于Windows版本的说明

作者使用了PowerShell脚本（*.ps1）来实现Windows的功能，已经在1.1.0中发布
