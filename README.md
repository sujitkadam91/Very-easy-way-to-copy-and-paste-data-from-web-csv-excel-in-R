### Very-easy-way-to-copy-and-paste-data-from-web-csv-excel-in-R
Very easy way to copy and paste data from web, csv, excel file by using (datapasta) and (reprex) packages in R 

#Subscribe this YouTube Channel Data/Fun



install.packages(datapasta)
install.packages(reprex)
library(datapasta)
library(reprex)



#From CSV/Excel

data_set<- tibble::tribble(
  ~Retailer.country, ~Order.method.type,  ~Retailer.type,       ~Product.line,   ~Product.type,                    ~Product, ~Year,  ~Quarter,  ~Revenue, ~Quantity, ~Gross.margin,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",  "Cooking Gear", "TrailChef Deluxe Cook Set", 2012L, "Q1 2012",  59628.66,      489L,    0.34754797,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",  "Cooking Gear",    "TrailChef Double Flame", 2012L, "Q1 2012",  35950.32,      252L,     0.4742745,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",         "Tents",                 "Star Dome", 2012L, "Q1 2012",  89940.48,      147L,    0.35277197,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",         "Tents",              "Star Gazer 2", 2012L, "Q1 2012", 165883.41,      303L,    0.28293788,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment", "Sleeping Bags",           "Hibernator Lite", 2012L, "Q1 2012",  119822.2,     1415L,    0.29145017,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment", "Sleeping Bags",        "Hibernator Extreme", 2012L, "Q1 2012",  87728.96,      352L,    0.39814629,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment", "Sleeping Bags",       "Hibernator Camp Cot", 2012L, "Q1 2012",  41837.46,      426L,    0.33560737,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",      "Lanterns",              "Firefly Lite", 2012L, "Q1 2012",   8268.41,      577L,    0.52896022,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",      "Lanterns",           "Firefly Extreme", 2012L, "Q1 2012",    9393.3,      189L,    0.43420523,
    "United States",              "Fax", "Outdoors Shop", "Camping Equipment",      "Lanterns",           "EverGlow Single", 2012L, "Q1 2012",   19396.5,      579L,    0.46149254
  )


data_set

sum(data_set$Revenue)


#From website

movie_data<- tibble::tribble(
  ~V1,                                     ~V2,    ~V3,            ~V4,   ~V5,            ~V6,   ~V7,     ~V8,     ~V9,
   1L,                         "Black Panther",   "BV", "$700,059,566",  4084, "$202,003,951",  4020,  "2/16",   "8/9",
   2L,                "Avengers: Infinity War",   "BV", "$678,815,482",  4474, "$257,698,183",  4474,  "4/27",  "9/13",
   3L,                         "Incredibles 2",   "BV", "$608,443,207",  4410, "$182,687,905",  4410,  "6/15",     "-",
   4L,        "Jurassic World: Fallen Kingdom", "Uni.", "$416,769,345",  4485, "$148,024,610",  4475,  "6/22",  "10/4",
   5L,                            "Deadpool 2",  "Fox", "$318,491,426",  4349, "$125,507,153",  4349,  "5/18", "10/18",
   6L,         "Mission: Impossible - Fallout", "Par.", "$220,159,104",  4395,  "$61,236,534",  4386,  "7/27", "10/18",
   7L,                  "Ant-Man and the Wasp",   "BV", "$216,648,740",  4206,  "$75,812,205",  4206,   "7/6",  "11/1",
   8L,               "Solo: A Star Wars Story",   "BV", "$213,767,512",  4381,  "$84,420,489",  4381,  "5/25",  "9/20",
   9L,                          "Venom (2018)", "Sony", "$210,782,620",  4250,  "$80,255,756",  4250,  "10/5",     "-",
  10L,                         "A Quiet Place", "Par.", "$188,024,361",  3808,  "$50,203,562",  3508,   "4/6",   "8/2",
  11L,                 "A Star is Born (2018)",   "WB", "$187,475,173",  3904,  "$42,908,051",  3686,  "10/5",     "-",
  12L,                     "Crazy Rich Asians",   "WB", "$173,765,895",  3865,  "$26,510,140",  3384,  "8/15",     "-",
  13L, "Hotel Transylvania 3: Summer Vacation", "Sony", "$167,485,460",  4267,  "$44,076,225",  4267,  "7/13",     "-",
  14L,                      "Halloween (2018)", "Uni.", "$158,945,295",  3990,  "$76,221,545",  3928, "10/19",     "-",
  15L,          "Dr. Seuss' The Grinch (2018)", "Uni.", "$145,471,250",  4141,  "$67,572,855",  4141,  "11/9",     "-"
  )

movie_data

Data_names <-c("Rank",	"Movie Title","Studio","Total Gross","Total Gross/Theaters","Opening","Opening/Theaters","Open","Close")

colnames(movie_data)<-Data_names ## for changing col names


movie_data

#Subscribe this YouTube Channel Data/Fun
