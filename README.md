
# SumIssueSumFile

`SumIssueSumFile(issue, file, target_dir)`
list the sumtree output, the issue we are working on, and the entire 
current file, along with a json yes/no dialog for if the current file 
is pertinent to our issue; returns true or false

## example run

So we're manageing a context-management-workflow, where we have 
several tasks that constitute the job.

We are acting as a middleman interaction between a large set of senior and junior developers

### frontmatter:

```
[-] cd to target_dir
[+] output of `sumtree ./`
[+] issue_content
```

### environment-info:

```
[-] env.nix
[-] libs.json
[+] print_version_info.txt
```

### issue:

```
[-] env.nix
[-] issue.sh
[+] verbose_log_of_running_issue.sh.txt
```

Our job as an assistant is to make sure the above tasks will be running as needed according to 

VLORI or verbose_log_of_running_issue.sh.txt is the result of the .sh commands used to run all said programs, only we will have access to the files tagged with [-]

We are going to go through each command in VLORI

and if it is a file in our project we will mark the file as request_pertinence()

if it is not within our project we will not mark it for the junior devs to request_pertinence()

The junior-devs will be making the final decision if the senior-devs need to see the files to solve the issue we are working on.

before we can run the fixes from the senior-devs we need to prepare the compressed issue, help me edit the pertinent issues options on the files.json that controls which files are sent to the junior-devs for pertinence review.

remember only select files that directly print to VLORI.
