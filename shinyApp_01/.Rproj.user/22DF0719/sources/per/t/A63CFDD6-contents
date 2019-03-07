shinyUI(
  
  pageWithSidebar(
    headerPanel("My First Shiny App"),
    
    sidebarPanel(
      selectInput("Distribution", "Please select Distribution Type",
                  choices = c("Normal", "Exponential")),
      sliderInput("sampleSize", "Please select sample size: ",
                  min = 100, max = 5000, value = 1000, step = 100),
      conditionalPanel(condition = "input.Distribution == 'Normal'",
                       textInput("mean", "Please select the mean", 10),
                       textInput("sd", "Please select Standard Deviation", 3)),
      conditionalPanel(condition = "input.Distribution == 'Exponential'",
                       textInput("lambda", "Please select Exponential Lambda: ", 1))
    ),
    
    mainPanel(
      plotOutput("myPlot")
    )
    
  )
  
  
  

  
  
)