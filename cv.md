# Slava Ivanov
### Front-end Developer student
___

#### Contacts

- **Location:** Taganrog, Russia
- **Phone:** +7 (988) 568-72-36
- **Email:** drumtrack@yandex.com
- **GitHub:** [questrator](https://github.com/questrator)

___

#### About me:

I am currently working as a content manager and site administrator.
I plan to become a frontend developer.
Wish me luck :smile:

___

#### Skills and Proficiency:

- HTML & CSS
- JavaScript
- React (basics)
- Node.js (basics)
- Git, GitHub
- Adobe Photoshop

___

#### Code example:

**Snail Sort** kata from CodeWars ([link](https://www.codewars.com/kata/521c2db8ddc89b9b7a0000c1 "Snail Sort kata"))

> Given an `n x n` array, return the array elements arranged from outermost elements to the middle element, traveling clockwise.
>>```JS
>>array = [[1,2,3],
>>          [4,5,6],
>>          [7,8,9]]
>>snail(array) -> [1,2,3,6,9,8,7,4,5]
>>```
> This image will illustrate things more clearly:
>![Snail Sort kata illustration](http://www.haan.lu/files/2513/8347/2456/snail.png "Snail Sort kata illustration")
>

**My solution:**

```JavaScript
function snail(array) {
  let result = [];
  let k = array.length;
  for (let i = 0; i < k / 2; i++) {
    result.push(...array[0]);
    array.shift();
    for (let j = 0; j < array.length - 1; j++) {
      result.push(array[j][array[j].length-1]);
      array[j].pop();
    }
    if (array.length == 0) break;
    result.push(...array[array.length - 1].reverse());
    for (let j = array.length - 2; j >= 1 ; j--) {
      result.push(array[j][0]);
      array[j].shift();
    }
    array.pop();
  }
  return result;
}
```

___

#### Courses:

- RS Schools Course «JavaScript/Front-end. Stage 0» (*in progress*)

___

#### Languages:

- Russian (*native*)
- English (*B1*)