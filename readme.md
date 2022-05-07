function play(question, answer){
    var score =0;
    var readLineSync=require("readLine-sync");
    var userAnswer = readLineSync.question(question);
    if(userAnswer===answer){
      console.log("right");
      score++
    }
    else{
      console.log("wrong");
    }
    
    console.log(score);                            
  }
 
  var questions= [
    {
      question: "What I am pursuing for my graduation?    ",
      answer: "B.tech",
    },
    {
      question: "What is the name of my college?  ",
      answer: "GRD Institute",
    },
    {
     question:"Where do I live now?    "  ,
     answer: "Dehradoon",
    },
    {
      question:"What is my birthday month?  ",
      answer: "May",
    },
    {
      question:"What is my home town?   ",
      answer:"Dhampur",
    }, 
  ];
  for(var i=0; i<questions.length;i++){
    currentQuestion=questions[i];
    play(currentQuestion.question,currentQuestion.answer);
  }