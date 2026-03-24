## Overview
This process occurs daily on its own, retrieves the 10 most recent unread emails from the Gmail Primary inbox, sends each email to an AI model using OpenRouter, and assigns a classification to one of 4 labels. Depending on the classification, the appropriate Gmail label is applied, the email marked as read, and the email ID saved to MongoDB so that no email is ever repeated in the process.

No more tedious email sorting for you! Your inbox now organizes itself!

## What it does
# Reads 10 unread Gmail emails daily
# AI classifies each email into 4 categories
# Adds Gmail label automatically
# Deletes spam emails from inbox
# Marks all processed emails as read
# Saves processed IDs to MongoDB
# Skips duplicate emails automatically

## What you need
# n8n (self-hosted v2.12+)
# Gmail account with OAuth2
# OpenRouter account + API key
# MongoDB Atlas account (free tier)
# Gmail labels: Action, Informational, Receipt


## Problem
Any professional gets between 50 to 100+, and sometimes more, emails in a day. It is a waste of 30 to 60 minutes a day to go through all of them to determine what is important and what is not. Important emails get lost in a sea of newsletters, promotions, and spam messages. Deadlines, invoices, and reply-to emails are often overlooked.

## Agitate
Every day you open Gmail and are overwhelmed by the number of emails in your inbox. Manually scroll through them, open them, read them, and decide on them 50 times a day. Your important client emails are mixed with other emails from Freelancer job postings, MongoDB emails, and Facebook notifications. When you finally manage to get to the important emails, you realize that you have already wasted an hour and are no longer in the right frame of mind.

## Solution
This n8n workflow operates on its own every day. It reads all your emails, sends them to AI, and in seconds, all emails are sorted, labeled, and organized. You open Gmail and only see what’s important. Tasks are flagged, receipts are filed, and spam is deleted. Email now takes 2 minutes a day instead of 60