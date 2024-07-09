AI Cloud utilizes [Ceph](https://docs.ceph.com/) as its storage solution, providing a robust and scalable file system for your data needs. Your files are organized within the Ceph file system hierarchy, ensuring efficient access and management across the entire platform.

<hr>

## User Directory
Your user directory serves as the primary location for storing personal files and data. It is structured within the Ceph file system as follows:

<div class="tree">
    <ul>
    <li><i class="fa fa-folder-open"></i> / <span>AI Cloud's file system</span>
        <ul>
        <li><i class="fa fa-folder-open"></i> home <span>user home directories</span>
            <ul>
            <li><i class="fa fa-folder-open"></i> [domain] <span>e.g student.aau.dk</span>
                <ul>
                    <li><i class="fa fa-folder"></i> [user] <span>your user directory</span></li>
                </ul>
            </li>
            </ul>
        </li>
        </ul>
    </li>
    </ul>
</div>

Here, [domain] represents your domain or institution (e.g., student.aau.dk), and [user] denotes your unique username on the platform. Any files you store within your user directory are private.

<hr>

## Shared Project Directories
AI Cloud fosters collaborative work through shared project directories. These directories enable multiple users to collaborate on projects by providing a centralized space for data sharing and collaboration. Shared project directories are organized under the project directory within the Ceph file system:

<div class="tree">
    <ul>
    <li><i class="fa fa-folder-open"></i> /home <span>AI Cloud's file system</span>
        <ul>
        <li><i class="fa fa-folder-open"></i> project <span>shared project directories</span>
            <ul>
            <li><i class="fa fa-folder"></i> project_X
            </li>
            </ul>
        </li>
        </ul>
    </li>
    </ul>
</div>

Your projects directory is a subdirectory to an overall project directories folder hierarchy.

Go in to the project directory

```
cd /home/project
```

Before going ahead and creating a directory for group project, please consider naming the directory in a meaningful manner (ie. after your group or research project) A project directory can be created in the following manner (swap out `<name>` for the actual name of your project).

```
mkdir <name> 
```

Please remember, that these directories should be deleted when your project is finished, and you no longer need them. They are not intended for long term data storage.

Happy computing!

## Storage quota expansions
When users log in to AI Cloud for the first time, a user directory is created for them. These directories are allocated 1 TB of storage by default. This should be plenty for most users, but should you need additional space, it is possible to apply for storage quota expansions for a limited time using our [Storage quota expansions form](https://forms.office.com/e/AjT0GccAPb).

!!! info
    When you log in to the platform, you can see your storage usage of the user directory at the very top line:

    ```
    Current quota usage: 181GiB / 1.0TiB
    Welcome to Ubuntu 20.04.6 LTS (GNU/Linux 5.4.0-169-generic x86_64)

    * Documentation:  https://help.ubuntu.com
    * Management:     https://landscape.canonical.com
    * Support:        https://ubuntu.com/pro

    System information as of Fri Mar 15 11:09:21 CET 2024
    ```