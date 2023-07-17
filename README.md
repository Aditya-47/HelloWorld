// Prompt the user to enter their name
const name = prompt("Enter your name:");
//Display Message
console.log("Welcome to Github", name);

Scanner myObj = new Scanner(System.in);

System.out.println("****MENU****");
System.out.println("Choose between the following 2 commands");
System.out.println("1 for Factorial")
System.out.println("2 for Maximum Value")
System.out.println("Choose a function")
ch = myObj.nextInt();
			switch(ch)
			{
			case 1:
				factorial();
				break;
			case 2:
				findMax();
            }

// Function to calculate the factorial of a number
function factorial(num) {
  if (num === 0 || num === 1) {
    System.out.println("1");
  } else {
    System.out.println(num * factorial(num - 1));
  }
}

// Function to find the maximum value in an array
function findMax(arr) {
  let max = arr[0];
  for (let i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
      max = arr[i];
    }
  }
  System.out.println( max);
}
