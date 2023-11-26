The `time` module in Python provides functionalities for working with time-related operations. Here are some common uses of the `time` module:

1. **Sleep Functionality:**
   - The `time.sleep()` function is used to introduce a delay in the execution of the program. It takes the number of seconds as an argument, causing the program to pause for that duration.

   ```python
   import time

   print("This is printed immediately.")
   time.sleep(2)  # Pause execution for 2 seconds
   print("This is printed after a 2-second delay.")
   ```

2. **Measuring Execution Time:**
   - You can use `time` to measure the execution time of a code block. This is often helpful for performance analysis.

   ```python
   import time

   start_time = time.time()

   # Code block to measure execution time
   # ...

   end_time = time.time()
   elapsed_time = end_time - start_time
   print(f"Execution time: {elapsed_time} seconds")
   ```

3. **Formatted Time:**
   - The `time.strftime()` function is used to format time as a string according to a specified format.

   ```python
   import time

   current_time = time.strftime("%Y-%m-%d %H:%M:%S")
   print(f"Current time: {current_time}")
   ```

4. **Getting Current Time:**
   - The `time.time()` function returns the current time in seconds since the epoch (January 1, 1970). This is often used for timestamping.

   ```python
   import time

   current_time = time.time()
   print(f"Current timestamp: {current_time}")
   ```

5. **Calendar Operations:**
   - The `time` module provides functions like `time.localtime()` and `time.gmtime()` to convert timestamps to struct_time objects, which can be further used for calendar operations.

   ```python
   import time

   current_time = time.time()
   local_time = time.localtime(current_time)
   print(f"Local time: {local_time}")
   ```
