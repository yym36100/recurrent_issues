# recurrent_issues

// disable printf buffering in newlib
#include <stdio.h>
    // Disable buffering for stdout
    setvbuf(stdout, NULL, _IONBF, 0);
