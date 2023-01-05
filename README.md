# workflow-sandbox
Sandbox for testing GitHub Actions logic / syntax 
 
## Useful links:
- https://github.blog/changelog/ - Keep track of new features
- https://github.com/orgs/community/discussions - Community and discussion/support
- https://docs.github.com/en/actions - GitHub Docs - Official documentation
- https://skills.github.com/#automate-workflows-with-github-actions - Guide/training 
- https://docs.ansible.com/ansible/latest/reference_appendices/YAMLSyntax.html - YAML syntax
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet - Markdown Cheatsheet
 
----
 
## Troubleshooting 
### Dump Context
To logg the [GitHub Context](https://docs.github.com/en/actions/learn-github-actions/contexts), use the action in _.github/actions/DumpContext_, you can call the action (NOTE use limited to this repo) from your workflow using:
 
    - name: 'Dump GitHub context'
      uses: ./.github/actions/DumpContext
      
### env
The env context contains environment variables that have been set in a workflow, job, or step. To logg these, use:
 
    - name: 'Log env context'
      run: env
