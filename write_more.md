# Lessons from The Elements of Data Science Analytics: 1-10

I’m currently going through this book list by Dataquest (though I’m not planning to read all of them). And I’ve just finished reading my first book: The Elements of Data Science Analytics by J Leek.

To practice sharing the things I’ve learned, I’ll be summarising some pertinent lessons from the book in this post. I’m not going to write all the lessons here or it’ll be too long. They’ll be in multiple posts instead.

Or if you would like to read something much much better than my writeup, read the author’s course notes which cover the same thing I’m about to share. He also has a wonderful list of links to his other course notes here. 

Or just read the book instead. It’s a Pay What You Want book with the minimum being FREE (yes, you also don’t need to “pay” with your email and join a mailing list). Still, you’ll have to s
register for an account with LeanPub, the publisher, but that’s necessary for them to keep track and make your purchases accessible in one place e.g. in case you lose the download link.

Anyhow, let’s go.

—-

Lesson 1: Always define the data analytic question first

As much fun as it is to just jump in and do some statistical analysis, it is wiser to restrain that excitement for awhile and define the questions first. 

The author listed six types of data analytic questions and they are listed in order of their simplicity and ability to determine causal relationships.

The six question types:

1. Descriptive
2. Exploratory
3. Inferential
4. Predictive
5. Causal
6. Mechanistic

Instead of having separate examples for each question, let’s use Dataquest’s Helicopter Escape project as the base example for all question types.

### 1. Descriptive

A descriptive data analysis is the summarization of the measurements within the data set without further interpretation. Though, try not to over-interpret the “without further interpretation” part: it’s just saying that descriptive analysis is fairly simple and if you find yourself struggling, it’s likely you’re trying to answer an even more difficult question or there’s something wrong with the data. For example, when conducting a descriptive data analysis, you might describe the data set’s size or shape, or a measurement’s mean, median, frequencies, and so forth. Any further interpretation will make it more exploratory rather than merely descriptive.

Let’s use the helicopter escape attempts example. Descriptive questions for that topic can  be:

1. What is the total number of helicopter escape attempts so far?
2. Which country has the highest number of helicopter escape attempts?
3. Which year has the highest number of helicopter escape attempts?
4. How many inmates had escaped from prison by a helicopter more than once?
5. What’s the average number of helicopter escape attempts per year?

### 2. Exploratory

Exploratory is about finding relationships between measurements. A simple form of this is to take two measurements and plot how a change in one measurement in response to a change in another. 

For helicopter escapes, exploratory questions could be:

1. Is there a relationship between the country a prison is located and the number of helicopter escapes?
2. Is the number of helicopter escapes increasing every year?
3. Does the number of escapees affect helicopter escapes chances of success?

### 3. Inferential

Inferential analysis tries to infer whether relationships observed in one data set can be seen in a different data set/context. Note that inferential analysis doesn’t try to predict a specific measurement; it merely looks for pattern similarities between multiple data sets.

Imagine that the helicopter escape data set is split into two: one for France and one for non-France. Now, we can ask inferential questions:

1. In France, helicopter escapes are more successful when there are more escapees. Is that the same in other countries?
2. In France, those who successfully escaped by a helicopter are normally caught within a month from the escape date. Is that the same in other countries?

*Note that the above are made-up and not actual facts about helicopter escapes in France.*

### 4. Predictive

Predictive analysis tries to predict a measurement based on another measurements. Unlike inferential analysis, it is less interested in quantifying relationships between two measurements, but more interested in predicting a specific measurement by using other measurements.

With helicopter escapes, potential predictive questions could be:

1. Can we predict the success a helicopter escape based on the number of escapees?
2. If there are 3 escapees and they’re all Americans, can we predict if the escape would be successful?
3. Based on what we know about a prison’s current security, can we predict if a helicopter escape attempt will happen this year?

### 5. Causal

Causal analysis investigates changes in one measurement when another measurement changes. This is normally tied to experiments and is the only one (aside from mechanistic analysis) that can indicate causality. 

If you’ve been in the data science world for some time, you’ll often hear people saying “correlation is not causation”. One reason why that statement is always uttered is when we’re unaware, we tend to be careless and use causal language to describe the results of non-causal analysis. Here’s a nice infographic showing a list of causal and non-causal words.

I’m going to stretch the helicopter escape example even further here.


http://jtleek.com/ads2020/week-1.html#types-of-data-analytic-questions

Image from above

Use DQ Helicopter Escape example to progressively show different data analytic questions
