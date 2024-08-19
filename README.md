COVID-19 Statistics Image Generator

This project is a Python script designed to generate dynamic images displaying COVID-19 statistics for the Kathmandu Valley. The script processes data such as new cases, recoveries, deaths, and district-wise breakdowns, and overlays them onto pre-designed templates. The result is a set of visually appealing, shareable images that provide an engaging and easy-to-interpret snapshot of the COVID-19 situation.
Features

    Dynamic Data Visualization: The script calculates daily changes in key COVID-19 statistics and displays them with color-coded indicators.
    District-wise Breakdown: It provides a detailed breakdown of cases for districts like Kathmandu, Lalitpur, and Bhaktapur.
    Customizable Fonts and Layout: The script uses different fonts and layout adjustments to ensure the data is presented clearly and aesthetically.
    Automated Image Generation: The final images are automatically generated and saved, ready to be shared or used in reports.

Requirements

    Python 3.x
    PIL (Python Imaging Library)
    A font file (sb.otf) for custom text rendering

Installation

    Clone the repository:

    bash

git clone https://github.com/yourusername/covid19-image-generator.git
cd covid19-image-generator

Install the required libraries:

bash

    pip install pillow

    Add the font file:
        Ensure the font file (sb.otf) is placed in the same directory as the script.

Usage

    Prepare the data:
        Update the dictionary with the latest COVID-19 statistics for Kathmandu, Lalitpur, and Bhaktapur.
        Provide the required parameters such as today's PCR count, new cases, recovered cases, and deaths.

    Run the script:

    python

    python script_name.py

    View the output:
        The script generates and displays the images automatically.
        The images are also saved in the current directory.

Example Code

Here's a snippet of the core function used to generate the images:

python

def printimage(dictionaryof, todaypcr, contaminatedpercent, newcases, recoveredcases, death, yesterdayinfected,
               yesterdayrecovered, yesterdaydead, yesterdaypcr, yesterdaypercent):
    image = Image.open("covidtry.jpg").convert('RGB')
    image2 = Image.open("covid3.jpg").convert('RGB')
    ...
    image.show()
    image2.show()
    image.save(filename)
    image2.save(filenamesecond)

Contributing

Feel free to fork this repository and submit pull requests for improvements or additional features. All contributions are welcome!
License

This project is licensed under the MIT License. See the LICENSE file for details.
Contact

For any questions or suggestions, please open an issue or reach out to your_email@example.com.
