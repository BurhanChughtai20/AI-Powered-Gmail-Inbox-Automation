## Overview
This is an automated workflow that runs daily, retrieving your 10 most recent unread emails from your Gmail Primary inbox, sending them to an AI model via Open Router, and applying one of 4 labels to them. Depending on the label, it adds a Gmail label, marks it as read, and saves the email ID to MongoDB to avoid processing an email twice.

No more manual sorting! Your inbox is self-organizing!

## What it does
# Reads 10 unread Gmail emails daily
# Classifies each email using AI into 4 categories
# Automatically labels the email using Gmail
# Deletes spam emails from inbox
# Marks all processed emails as read
# Saves processed email ids to MongoDB
# Skip reading duplicate emails

## What you need
# n8n (self-hosted v2.12+)
# Gmail account with OAuth2
# OpenRouter account + API key
# MongoDB Atlas account (free tier)
# Gmail labels: Action, Informational, Receipt

## Problem
Any professional receives between 50 and 100+ emails every day. Going through all the emails to decide which ones need attention wastes 30-60 minutes every day. Important emails may go unnoticed among newsletters, advertisements, and spams. Deadlines, invoices, and replies may go unnoticed.

## Agitate
Every morning, you log in to your Gmail account. You scroll through your inbox, open messages, read them, and respond. This process repeats for 50 emails. Important emails from your client are mixed with recommendations from Freelancer. MongoDB notifications are mixed with Facebook notifications. You are done reading your important emails in an hour. Your focus is gone.

## Solution
This workflow for n8n runs daily automatically. It scans your emails, sends them to AI, and in seconds, all your emails are sorted, labeled, and cleaned. You open your Gmail and only see what’s important. Your action items are flagged. Your receipts are filed. Your spam is gone. You now spend 2 minutes on email, not 60