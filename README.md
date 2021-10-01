 test machine: CSELAB_machine_name
 date: 10/09/19
 name: Orion Grebe, [full_name2]
 x500: grebe013, [id_for_second_name]


# 4061_project1
project 1 for 4061

Purpose:
  - to parse through a makefile, retrieve the targets, dependencies,
    and recipes, then based on user input, print the information to
    do with those to the terminal or execute their recipes.

Compile:
  - Simply ender gcc main.c into the terminal and hit enter.

To specifically get into what the project does:
  - process_into_objects()
    - processes the file from the user after going through process_file
      into a linked list of target objects.
  - p_function()
    - has helper functions
      - p_function_helper(target makefile)
    - prints the target's, how mant dependencies and recipes they have, as
      well as the names of them. Format is as follows.
        target ’all’ has 2 dependencies and 1 recipe
          Dependency 0 is dep1
          Dependency 1 is dep2
          Recipe 0 is ls -l
  - r_function()
    - has helper functions
      - make_block(char* name)
      - r_help(char** targets, int targ, int * target_hit, int tcount,int dcount)
    - prints the recipes of the makefile in order of need for execution
  - execute()

Assumptions:
  - lines either started with a /t character or a regular character
  - lines ended with NULL

Orion contributions:
  - programmed process_into_objects()
  - programmed p_function()
  - programmed main()
Sami contributions
  - programmed r_function()
  - programmed execute()
