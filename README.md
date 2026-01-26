# recurrent_issues

// disable printf buffering in newlib
#include <stdio.h>

    // Disable buffering for stdout
    
    setvbuf(stdout, NULL, _IONBF, 0);
//ram soft reset

monitor reset
load

memdump to file
dump binary memory dump.bin 0x20000000 0x20010000
dump binary memory buf.bin &my_buffer (&my_buffer + sizeof(my_buffer))

inspect
p &my_buffer
p sizeof(my_buffer)

https://chatgpt.com/share/69771d81-fba8-800e-abf3-5916e9aaec29

		dump binary memory app_buf.bin &app_buf (&app_buf + sizeof(app_buf))
		dump binary memory app_buf.bin &app_buf $end
		
		set $end   = (char*)&app_buf + sizeof(app_buf)


        

