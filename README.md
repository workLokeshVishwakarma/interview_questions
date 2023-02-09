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
              
### 2). Question
### Reverse entire 2d array javascript
- <i>Solution</i>
    - #### 1).
          const N_Arr = [[1,2,3], [4,5,6], [7,8,9]]
          console.log(N_Arr.map(p_arr => p_arr.reverse()).reverse());
              
    - #### 2).
          const N_Arr = [[1,2,3], [4,5,6], [7,8,9]]
          const reversed_N_Arr = []
          for (let i = N_Arr.length-1; i >= 0; i--) {
              const temp = []
              for (let j = N_Arr[i].length-1; j >= 0; j--) {
                  temp.push(N_Arr[i][j])
              }
              reversed_N_Arr.push(temp)
          }
          console.log(reversed_N_Arr);
              
