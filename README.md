## Memory leak deomonstartions

Dear Developers of this channel & and anyone reading this, I am sharing the problems faced while working on a project. I've tried to recreate the possible memory leak issue. To present here and give an idea of these kinds of problems, I have removed few pages which from the navigation menu in the navbar.

Firstly, I am new on stack blitz and somehow this project here is not loading the homepage initially, so one has to start with the url mentioned below:

/news-and events

a.)After that, to recreate the memory leeak issue, you have to go back and forth on News & Events and then to Home and vice-versa.
b.)You can try toggle the Tender droop down on the navbar and then navigate to news and events
c.) Heap Snapshot

If you take a heap snapshot then you'll be able to see an increase of size by somewhat around 1 to 3 MBs. Doing the (a),(b),(c) steps again and again will lead to a lot of memory.

For demo purpose I've trimmed off few pages but If all the pages, iamges and components are present and I do these steps then I get a lot approximately ~4-10 MB.This issue is mostly noticed when I go from home to any page and back to home. I see a lot of Detached elements.

I will attach some screenshots via an external link below for the recreated website on stackblitz

On Stackblitz

(Link to the album containing all 5 screenshots)['https://ibb.co/album/CbQVVh']

(Screenshot 1)['https://ibb.co/b7NTjZj']
(Screenshot 2)['https://ibb.co/Z6fdFFq']
(Screenshot 3)['https://ibb.co/s9h2cH8']
(Screenshot 4)['https://ibb.co/mDvqrPx']

I look forward for help from you all and wish to resolve this issue.

Thanks dear
