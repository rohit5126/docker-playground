# Docker Command Cheat Sheet

## Common Commands:

  `run         Create and run a new container from an image`

  |OPTIONS| USAGE |
  |---------|-----------|
  -a | add a custom host-to-IP mapping
  -d   | detach mode
  -e | set environment variable
  -h | conatiner hostname
  -i | Keep STDIN open even if not attached
  -l | Set meta data on a container
  -m | memory limit
  -p | port mapping
  -t | Allocate a pseudo-TTY
  -u | user and UID
  -v | volume mapping 
  -w | Working directory inside the container
  ------------------------------- 
  
  `exec        Execute a command in a running container`               
  ### docker exce -it frontend bash**
 ---------------------------------------- 
  `ps          List containers`
  |OPTIONS| USAGE |
  |---------|-----------|
  |-a   |    Show all containers (default shows just running)
  |-f  |  Filter output based on conditions provided
  |-n |        Show n last created containers (includes all states) (default -1)
  |-l |        Show the latest created container (includes all states)    
  | -q |           Only display container IDs
  | -s |       Display total file sizes
----------------------------------
  
  `build       Build an image from a Dockerfile`
  |OPTIONS| USAGE |
  |---------|-----------|
  -c  | CPU shares
  -f  | dockerfile name
  -m  | memory limit
  -t  | Name and optionally a tag in the "name:tag" format
  -q  | Suppress the build output and print image ID on success
  ------------------------------------
  
  `pull        Download an image from a registry`   
   
   |-a       | Download all tagged images in the repository
   |---------|-----------|
  ### docker pull -a rohit5126/devboard-frontend

----------------------------------
  
  `push        Upload an image to a registry`
  
  |-a       | Download all tagged images in the repository
  |---------|-----------|
  ### docker push -a rohit5126/devboard-frontend
  -------------------------------------
  
  `images      List images`
  
  |OPTIONS| USAGE |
  |---------|-----------|
  |-a  |            Show all images (default hides intermediate images)
  |-f  |   Filter output based on conditions provided
  | -q |         Only show image IDs
  --------------------------------------
  ### docker login
  `login       Authenticate to a registry`                             
  `logout      Log out from a registry`
  
  ------------------------------------
  `search      Search Docker Hub for images`                                   
  `version     Show the Docker version information`                                        
  `info        Display system-wide information`                        
  
-----------------------------------------
## Management Commands:

  `context     Manage contexts`
  
  |command| USAGE |
  |---------|-----------|
  create    |  Create a context
  export    |  Export a context to a tar archive FILE or a tar stream on STDOUT.
  import    |  Import a context from a tar or zip file
  inspect    | Display detailed information on one or more contexts
  ls         | List contexts
  rm          |Remove one or more contexts
  show        |Print the name of the current context
  update      |Update a context
  use         |Set the current docker context
  ---------------------------------------------
  
  `image       Manage images`
  |command| USAGE |
  |---------|-----------|
  history   |  Show the history of an image
  import    |  Import the contents from a tarball to create a filesystem image
  inspect   |  Display detailed information on one or more images
  load      |  Load an image from a tar archive or STDIN
  ls        |  List images
  prune     |  Remove unused images
  pull      |  Download an image from a registry
  push       | Upload an image to a registry
  rm         | Remove one or more images
  save       | Save one or more images to a tar archive (streamed to STDOUT by default)
  tag        | Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE

  `network     Manage networks`
  |command| USAGE |
  |---------|-----------|
  connect    | Connect a container to a network
  create    | Create a network
  disconnect | Disconnect a container from a network
  inspect   |  Display detailed information on one or more networks
  ls        |  List networks
  prune     |  Remove all unused networks
  rm        |  Remove one or more networks
  ---------------------------
  
  `volume    |  Manage volumes`
  |command| USAGE |
  |---------|-----------|
  create    |  Create a volume
  inspect   |  Display detailed information on one or more volumes
  ls        |  List volumes
  prune     |  Remove unused local volumes
  rm        |  Remove one or more volumes
  ----------------------------------
  
## Commands:

 |command| USAGE |
 |---------|-----------|
  attach   |  Attach local standard input, output, and error streams to a running container
  commit   |   Create a new image from a container's changes
  cp       |   Copy files/folders between a container and the local filesystem
  create    |  Create a new container
  diff      |  Inspect changes to files or directories on a container's filesystem
  events    |  Get real time events from the server
  export    |  Export a container's filesystem as a tar archive
  history   |  Show the history of an image
  import    |  Import the contents from a tarball to create a filesystem image
  inspect   |  Return low-level information on Docker objects
  kill      |  Kill one or more running containers
  load      |  Load an image from a tar archive or STDIN
  logs      |  Fetch the logs of a container
  pause     |  Pause all processes within one or more containers
  port      |  List port mappings or a specific mapping for the container
  rename    |  Rename a container
  restart   |   Restart one or more containers
  rm        |  Remove one or more containers
  rmi       |  Remove one or more images
  save      |  Save one or more images to a tar archive (streamed to STDOUT by default)
  start     |  Start one or more stopped containers
  stats     |  Display a live stream of container(s) resource usage statistics
  stop      |  Stop one or more running containers
  tag       |  Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top       |  Display the running processes of a container
  unpause    | Unpause all processes within one or more containers
  update     | Update configuration of one or more containers
  wait       | Block until one or more containers stop, then print their exit codes
  system     | view system details like space usage, events etc.
  ----------------------------------------------
