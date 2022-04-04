# Online_news_sql
its A certification Postgresql project using sql query to explore a database table called "articles" provided by datacamp
# project overview
Following the changes in working habits during the COVID pandemic, The local library has decided it is time to make the newspaper archives available online. They are not sure what the response will be so they are going to trial a new system on a small set of their data.

The library database has a table articles with a record of all articles published in the newspaper. However, the table will need some preparation before the library can use it in the new system. They would like to focus the initial trial on articles from 2014 and 2015 only, and for just one journalist whose ID in the database is 1754.

The final results should be sorted from earliest published date to the most recent published date.
# requirements
<th style="text-align:left;">Requirements</th>
<th style="text-align:left;">Data Type</th>
<th style="text-align:left;">Column Alias</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">Unique ID of each article, where the first 4 digits represents the journalist ID.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">article_key</td>
</tr>
<tr>
<td style="text-align:left;">Category of the article, in uppercase.  'Food &amp; Drink' and 'Wellness' should be collapsed  into a 'Lifestyle' category.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">category</td>
</tr>
<tr>
<td style="text-align:left;">Headline of the article, without the subtitle that appears after the colon (:).  For example, 'It Could Happen To You: A Story of SEC Overreach' becomes 'It Could Happen To You'.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">headline</td>
</tr>
<tr>
<td style="text-align:left;">Subtitles of the article, without the headline that appears before the colon (:). For example, 'It Could Happen to You: A Story of SEC Overreach' becomes 'A Story of SEC Overreach'. In cases where a headline does not have a subtitle, the missing value should read ‘None’.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">subtitle</td>
</tr>
<tr>
<td style="text-align:left;">Description of the article. The description should be reduced to the first sentence, up to and including the first period (.) from the short_description column.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">description</td>
</tr>
<tr>
<td style="text-align:left;">Keywords of the article. Multiple keywords will be seperated with a dash (-). If the keyword is missing, the value should read ‘Unknown’.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">keywords</td>
</tr>
<tr>
<td style="text-align:left;">Date the article was published. The data should be displayed in the format resembling the following: ‘Aug 13, 1995’.</td>
<td style="text-align:left;">TEXT</td>
<td style="text-align:left;">publish_date</td>
</tr>
</tbody>
</table>
