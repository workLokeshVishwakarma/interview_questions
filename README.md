### 1). Question
![image](https://user-images.githubusercontent.com/120416755/216376656-9f60056d-2158-4ce3-8230-b18353cb3c4b.png)
- <i>Solution</i>
    - #### 1).
          const dup_arr = [1,2,3,8,2,7,3,4];
          console.log([...new Set([1,2,3,8,2,7,3,4])]);
              
    - #### 2).
          const dup_arr = [1,2,3,8,2,7,3,4];
          for (let i = 0; i < dup_arr.length; i++) {
              for (let j = 0; j < dup_arr.length; j++) {
                  if (dup_arr[i] == dup_arr[j] && i != j) {
                      dup_arr.splice(j, 1)
                  }
              }
          }
          console.log(dup_arr);
              
