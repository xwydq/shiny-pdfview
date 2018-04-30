


library(shiny)
library(timevis)
# addResourcePath("pdfView", "/home/xuwy/projectJC/pdfView")


# Define UI for application that draws a histogram
ui <- fluidPage(
   
   # Application title
   titlePanel("pdf view"),
   
   # Sidebar with a slider input for number of bins 
   uiOutput("iframe_source")
)

# Define server logic required to draw a histogram
server <- function(input, output) {
  output$iframe_source <- renderUI({
  iframe_source = tags$iframe(
    src=sprintf("pdfView/generic/web/viewer.html?file=../../0b781915c086876a5eac6b1b30ba0d18.pdf"),
                              height=800, width='90%')
  iframe_source
  })
}

# Run the application 
shinyApp(ui = ui, server = server)

