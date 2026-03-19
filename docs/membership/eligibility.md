# Membership

## Membership Categories and Eligibility

See [here](apply.md) for the procedure to apply for membership

| No. | Membership | Eligibility | Fee  | Duration |
|:---:|:-----------|:------------|-----:|:---------|
| 1.  | Individual Life Membership | Postgraduate degree in strucural engineering (or allied programs) from a recognized University/Institute | Rs. 10,000 | Lifetime |
| 2.  | Institutional Membership | Institution employing postgraduate structural engineers | Rs. 25,000 | Lifetime |
| 3.  | Student Membership | Students enrolled in a postgraduate structural engineering (or allied) program in a recognized University/Institute | ₹ 500 | Duration of enrolment in a postgraduate structural engineering academic program |

[Download](membershipforms.md) membership application forms

**Note**

1. A recognized University/Institute is an Indian University/Institute that is recognised by [UGC](https://www.ugc.gov.in/), or an Institution of National Importance (such as IIT, NIT, IIIT, etc.)  or a foreign University recognized by the [Association of Indian Universities](https://aiu.ac.in/).
2. Student membership is restricted to the duration the student is enrolled in a postgraduate program in structural engineering
3. A postgraduate program allied to structural engineering includes programs such as Industrial Structures, Computer Aided Design of Structures, Earthquake Engineering etc. whose curriculum includes predominantly structural engineering courses

## Benefits
{% set mem_data = load_data(path="data/membership.csv", format="csv")%}
| No. | Membership | Eligibility | Fee  | Duration |
|:---:|:-----------|:------------|-----:|:---------|
{% for row in mem_data.items | slice(start=1) -%}
| {{ row[0] }} | {{ row[1] }} | {{ row[2] }} | {{ row[3] }} | {{ row[4] }} |
{% endfor %}