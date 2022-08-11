Contents:
	-EDA (folder)
		EDA_Shelter_Data (Tableau)
		Shelter_Data_Visuals (Tableau)

	-Notebooks and Data(folder)
		>Image Data (folder) - DELETED
			*images (folder)
			*output (folder)
				~train (folder)
				~val (folder)
				~test (folder)
			*input_file_resize (folder)
				~train (folder)
				~val (folder)
				~test (folder)
			
		>Tabular Data (folder)
			*all_records (csv)
			*austin_animal_center_intakes (csv)
			*austin_animal_center_outcomes (csv)
			*lost_found_adoptable_pets (csv)
			*EDA_austin_shelter_dog (csv)
			*num_austin_shelter_dog (csv)
			*new_adopt_category (csv)

		>1. Exploring Dog Adoption and Image Data (Jupyter Notebook)
		>2. Table Joining and Discovery (Jupyter Notebook)
		>3. Logistic Regression Statsmodel (Jupyter Notebook)
		>4. SKlearn Modeling (Jupyter Notebook)
		>5. Neural Network and Boosting (Jupyter Notebook)
		>6. Image Analysis (Jupyter Notebook)

	-Report (pdf)
	-Environment Setup (note pad)


Descriptions:
	-EDA (folder)
		1. EDA_Shelter_Data (Tableau)
			exploratory data analysis conducted after creating the 
			EDA_Austin_Shelter_Dog data frame in the Table Joining and Discovery 
			Jupyter Notebook to help chose the most important features
		2. Shelter_Data_Visuals (Tableau)
			final exploratory data analysis visuals created with the same
			EDA_Austin_Shelter_Dog data frame, but with more focus on meaningful
			independent variables

	-Notebooks (folder)
		>Image Data (folder)
		NOTE: this folder was deleted because the final project file
		submission size was too large
			*images (folder)
				contains 120 folders - one for each breed of dog - each folder 
				contains 150-250 images representative of each breed - images 
				are variant in location and coloring patterns and some contain
				humans
			*input_file_resize (folder)
				~train (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 40% of the images in the original "images"
					folder with the same title - each image is (100, 100, 3)
				~val (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 20% of the images in the original "images"
					folder with the same title - each image is (100, 100, 3)
				~test (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 40% of the images in the original "images"
					folder with the same title - each image is (100, 100, 3)
			*output (folder)
				~train (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 40% of the images in the original "images"
					folder with the same title
				~val (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 20% of the images in the original "images"
					folder with the same title
				~test (folder)
					contains 120 folders - one for each breed of dog - each 
					folder contains 40% of the images in the original "images"
					folder with the same title

		>Tabular Data (folder)
			*all_records (csv)
				CSV file downloaded from Kaggle containing Austin, Texas Animal
				Shelter data from both the "outcome" and "intake" data frames
				used in notebooks 1 and 2
			*austin_animal_center_intakes (csv)
				CSV file downloaded from Kaggle containing Austin, Texas Animal
				Shelter data focusing on intake conditions and animal description
				used in notebooks 1 and 2
			*austin_animal_center_outcomes (csv)
				CSV file downloaded from Kaggle containing Austin, Texas Animal
				Shelter data focusing on the outcome conditions and animal 
				description used in notebooks 1 and 2
			*lost_found_adoptable_pets (csv)
				CSV file downloaded from dataworld.com containing King County
				shelter data of rescued animals including the "adoptable" column, 
				conditions, and image of the animal - 409 rows - used in notebook 1
			*EDA_austin_shelter_dog (csv)
				CSV file output from notebook 2 with slightly cleaned data - 31133
				rows - used in Tableau visualizations
			*num_austin_shelter_dog (csv)
				CSV file output from notebook 2 - ready for modeling with the 
				target variable "outcome type" being adopted (1) versus all other 
				outcomes (0) - did not end up using this in modeling - 25624 rows
			*new_adopt_category (csv)
				CSV file output from notebook 2 - ready for modeling and used in 
				all future modeling notebooks with the target variable "outcome
				type" being adopted (1) and transferred (0) - 19349 rows

		>1. Exploring Dog Adoption and Image Data (Jupyter Notebook)
			Explores the basics of the 3 Austin, TX datasets (input, output, all) as
			well as the King County dataset with images
		>2. Table Joining, Cleaning, and EDA (Jupyter Notebook)
			Joins the 3 Austin, TX Shelter datasets, exploring each column in detail
			before cleaning appropriately and creating 3 new data frames: 1) EDA, 
			2) Adopted or Transferred/Euthanized, 3) Adopted or Anything Else
		>3. Logistic Regression Statsmodel (Jupyter Notebook)
			Fit logistic regression model using the Statmodels package on two different
			target variable splits and determines that the adopted versus moved to
			partner or euthanized is the dataset being used moving forward
		>4. SkLearn Modeling (Jupyter Notebook)
			Explores some Scikit-Learn models appropriate for this data and compares 
			accuracy, recall, and precision. Further explains what this means for the
			shelter. 
		>5. Neural Network and Boosting (Jupyter Notebook)
			Explores the predictive power of Neural Networks on this dataset and 
			briefly discusses how boosting might improve the model. 
		>6. Image Analysis (Jupyter Notebook)
			Quickly explores how well transfer learning can classify the breed of
			120 different kinds of dogs using 20,580 various images in the image
			folder discussed above.

	-Report (pdf)
		Highlights the findings the major findings of this project and outlines next steps
	-Environment Setup (note pad)
		Provides details on setting up the environment to run the notebooks within