# phoronix-ansible
First try to automate phoronix test suite, setup and one test.

Sorry, but currently tested only with CentOS 7

# Usage / use case
roles:
  
  - common # common for standard operations / install repo and yum install phoronix and deps
  
  - phoronix-install # configure phoronix and batch-install bench's
  
  - phoronix-bench # do instlled bench
  
  - phoronix-merge # once we have several bench'es we want to merge these to one report, which will be located on remote host /root dir, also do not forget to remove /var/lib/phoronix-test-suite/test-results/merge* once got your report. or remove VM :)

# Thank you goes to:
Domas Tamašauskas (co-worker)

zoredache - IRC help :) in FreeNode #ansible

agaffney - IRC help :) in FreeNode #ansible
