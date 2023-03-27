ParrotOS-like Prompt for Korn Shell
Copyright (c) 2023 by Luke C Dahlgren

This is a prompt that is compatible with AT&T Korn Shell and KSH93
Colors and font emphases are customizeable, using the pallete noted within the code comments.

NOTE: This assumes you have a dark terminal (i.e. black background, white text) and so the pallete is reset to regular white text at the end of the prompt, so that your actual prompt text will be white.  You may change this by 

The pallete is defined within the .prompt_colors script and usage is described in more detail in the .ksh_prompt file itself.

__Examples__

![parrot-ksh1](https://user-images.githubusercontent.com/89806345/228074930-1358133a-dd2d-42f6-b94b-ffd95e47e5b5.png)
![parrot-ksh2](https://user-images.githubusercontent.com/89806345/228074950-267475d7-b786-4b33-8510-675746fe48e5.png)
![parrot-ksh3](https://user-images.githubusercontent.com/89806345/228074962-b1b33f55-97b1-4904-ba47-063182414d4a.png)


Colors available in both regular *and* bright variants:
    - red
    - green
    - yellow
    - blue
    - cyan
    - purple
    - white

Font emphases available:
    - Regular
    - Bold
    - Highlighted


__Instructions For Use:__

    1. place these files either directly in your home directory, or in a subfolder.  *These are technically hidden files (preceded by .), so unless you enable viewing of hidden files in your file browser and/or ls -a in a terminal, you will not see them.  You can easily change this if you wish by removing the ".". If you do this to the .prompt_colors file, be sure to update the reference within the .ksh_prompt script!

    2. If desired, change the color scheme where indicated in the .ksh_prompt script.  Be sure to preserve the braces {} surrounding each color.

    3. Call the script from your ~/.kshrc, or manually if you wish...  I would recommend adding the following to your .kshrc resource file (if you have one, if not, you can create one).  Update reference as necessary:

        `if [ -f ~/.ksh_prompt ]; then
           . ~/.ksh_prompt
         fi`

    4. Enjoy!
